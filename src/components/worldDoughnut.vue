<template lang="pug">
#Planet-o-Doughnut.flex.flex-wrap.bg-white.h-auto
  .px-8(class='lg:block lg:w-1/2 sm:w-full')
    doughnut(:data="[10, 40, 15, 25, 50]")
  .flex.items-center.text-center.px-8.py-4(class='lg:text-right md:px-12 lg:w-1/2')
    h2.text-3xl.font-semibold.text-gray-800(class='md:text-4xl')
      span.text-indigo-600 Planet
      span -🌏-Doughnut Example
</template>

<script>
import { ref, onMounted } from 'vue';
import doughnut from "./doughnut.vue"

//import {Chart, DoughnutController, ArcElement, RadarController, RadialLinearScale, PointElement, LineElement, LineController, PolarAreaController, CategoryScale, LinearScale } from 'chart.js'
import {planetChartData, data} from './planet-data.js'
import * as d3 from "d3";


export default {
  name: 'navBar',
  components: {
    doughnut
  },
  
  setup() {
    let rootChart = ref(null)
    

    onMounted(() => {
      var dataset = [
          { label: 'Abulia', count: 10 }, 
          { label: 'Betelgeuse', count: 20 },
          { label: 'Cantaloupe', count: 30 },
          { label: 'Dijkstra', count: 40 }
        ];

        var width = 360;
        var height = 360;
        var radius = Math.min(width, height) / 2;
        var donutWidth = 75;                            // NEW

        console.log(rootChart)

        var svg = d3.select(rootChart)
          .append('svg')
          .attr('width', width)
          .attr('height', height)
          .append('g')
          .attr('transform', 'translate(' + (width / 2) + 
            ',' + (height / 2) + ')');

        var arc = d3.arc()
          .innerRadius(radius - donutWidth)             // NEW
          .outerRadius(radius);
          
        var pie = d3.pie()
          .value(function(d) { return d.count; })
          .sort(null);

        var path = svg.selectAll('path')
          .data(pie(dataset))
          .enter()
          .append('path')
          .attr('d', arc)
          .attr('fill', function(d, i) { 
            return color(d.data.label);
          });


     
      /*Chart.register(DoughnutController, ArcElement, RadarController , RadialLinearScale, PointElement, LineElement, LineController, PolarAreaController, CategoryScale, LinearScale)
      let ctx = rootChart.value.getContext('2d');
      rootChart.width = 320;
      rootChart.height = 240;
      const planetChartjs = new Chart(ctx,planetChartData);
      */

    })
    return{ rootChart }
  }
};
</script>

<style scoped></style>
