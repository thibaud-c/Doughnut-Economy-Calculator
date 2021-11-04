<template lang="pug">
navBar
.flex.bg-white(style='height:100px;')
landingBanner
.flex.bg-white(style='height:100px;')
worldDoughnut
.flex.bg-white(style='height:100px;')
projectInformation
.flex.bg-white(style='height:100px;')
team
.flex.bg-white(style='height:100px;')
bottomBar
</template>

<script>
import navBar from './components/navBar.vue';
import landingBanner from './components/landingBanner.vue';
import projectInformation from './components/projectInformation.vue';
import worldDoughnut from './components/worldDoughnut.vue';
import team from './components/team.vue';
import bottomBar from './components/bottomBar.vue';

export default {
  name: 'App',
  components: {
    navBar,
    landingBanner,
    projectInformation,
    worldDoughnut,
    team,
    bottomBar,
  },
};
</script>

<style>
#app {
  height: 100%;
}
svg {
  /* important for responsiveness */
  display: block;
  fill: none;
  stroke: none;
  width: 100%;
  height: 100%;
  overflow: visible;
  background: #eee;
}
</style>
