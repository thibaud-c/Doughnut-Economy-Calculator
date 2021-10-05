<template lang="pug">
bouton test
  <button>.button.is-info.is-light Join the waiting list</button>
  <img v-model="doughnut_parallax" class="thumbnail" src="/assets/images/doughnut_parallax.jpg" width='100'/>
  <figure class="image is-128x128">
    <img src="/assets/images/doughnut_parallax.jpg">
  </figure>
</template>

<script>
import { ref, onMounted } from 'vue';
import simpleParallax from 'simple-parallax-js';

export default {
  name: 'navBar',
  components: {},
  setup() {
    let doughnut_parallax = ref('');
    //onMounted(new simpleParallax(doughnut_parallax));

    return { doughnut_parallax };
  },
};
</script>

<style scoped></style>
