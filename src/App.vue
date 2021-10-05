<template>
  <navBar />
  <headSite />
  <bottomBar />
</template>

<script>
import navBar from './components/navBar.vue';
import headSite from './components/headSite.vue';
import bottomBar from './components/bottomBar.vue';

export default {
  name: 'App',
  components: {
    navBar,
    headSite,
    bottomBar,
  },
};
</script>

<style>
#app {
  height: 100%;
}
</style>
