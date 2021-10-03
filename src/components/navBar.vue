<template>
  <div class="tabs is-centered is-small">
    <ul>
      <li class="is-active"><a>Home</a></li>
      <li><a>Doughnut Calculator</a></li>
      <li><a>About us</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'navBar',
  components: {},
  setup() {
    const webSiteTitle = 'Doughnut Economy Calculator';

    return {
      webSiteTitle,
    };
  },
};
</script>

<style scoped>
#app {
  height: 100%;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}
</style>
