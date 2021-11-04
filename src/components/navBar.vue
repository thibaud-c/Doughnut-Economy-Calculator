<template lang="pug">
.w-full
  nav.bg-white.shadow-lg.flex.flex-col.flex-wrap.justify-center.text-base
    .items-center.justify-between.py-2.px-8(class='md:flex md:px-12')
      .flex.justify-between
        .text-2xl.font-bold.text-gray-800(class='md:text-3xl')
          a(href='#intro_section') The Doughnut🌍Meter
        #burgerMenu(class='md:hidden')
          button.block.text-gray-800(type='button', class='hover:text-gray-700 focus:text-gray-700 focus:outline-none')
            svg.h-6.w-6.fill-current(viewbox='0 0 24 24')
              path.hidden(d='M16.24 14.83a1 1 0 0 1-1.41 1.41L12 13.41l-2.83 2.83a1 1 0 0 1-1.41-1.41L10.59 12 7.76 9.17a1 1 0 0 1 1.41-1.41L12 10.59l2.83-2.83a1 1 0 0 1 1.41 1.41L13.41 12l2.83 2.83z')
              path(d='M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z')
      .hidden.-mx-2(class='md:block md:flex-row')
        a.text-gray-800.rounded.py-2.px-2(href='#Doughnut-Home', class='hover:bg-gray-900 hover:text-gray-100 hover:font-medium md:mx-2') Home
        a.text-gray-800.rounded.py-2.px-2(href='#Planet-o-Doughnut', class='hover:bg-gray-900 hover:text-gray-100 hover:font-medium md:mx-2') Planet🌍Doughnut
        a.text-gray-800.rounded.py-2.px-2(href='#The-Doughnut-Project', class='hover:bg-gray-900 hover:text-gray-100 hover:font-medium md:mx-2') Project
        a.text-gray-800.rounded.py-2.px-2.text-base(href='#Team-o-Doughnut', class='hover:bg-gray-900 hover:text-gray-100 hover:font-medium md:mx-2') Team
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
