<template lang="pug">
div(ref="resizeRef")
    svg(ref="svgRef")
</template>

<script>
import { onMounted, ref, watchEffect } from "vue";
import * as d3 from "d3";

import useResizeObserver from "./use/resizeObserver";

export default {
  name: "ResponsiveLineChart",
  props: ["data"],
  setup(props) {
    // create ref to pass to D3 for DOM manipulation
    const svgRef = ref(null);

    // this creates another ref to observe resizing, 
    // which we will attach to a DIV,
    // since observing SVGs with the ResizeObserver API doesn't work properly
    const { resizeRef, resizeState } = useResizeObserver();

    onMounted(() => {
      // pass ref with DOM element to D3, when mounted (DOM available)
      const svg = d3.select(svgRef.value);

      // whenever any dependencies (like data, resizeState) change, call this!
      watchEffect(() => {
        const { width, height } = resizeState.dimensions;

        var pie = d3.pie()
            .sort(null)
            .value(d => d.count);

        var arc = d3.arc()
            .innerRadius(Math.min(width, height) / 2 - 100)
            .outerRadius(Math.min(width, height) / 2 - 1)
            .cornerRadius(5);
        

        svg
        .attr("stroke", "white")
        .selectAll(".arc")
        .data(pie(props.data))
        .join("path")
            //
            
            //
            //.enter()
            //.append("path")
            //.attr("fill", d => "rgb(12,240,233)")
            //.attr("d", arc);

        })
    });

    // return refs to make them available in template
    return { svgRef, resizeRef };
  },
};
</script>
