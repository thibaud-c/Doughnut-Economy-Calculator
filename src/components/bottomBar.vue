<template lang="pug">
footer
  .container.mx-auto.py-4.px-5
    .flex.flex-wrap.items-center.flex-col.justify-center(class='md:justify-between sm:flex-row')
      .w-full.px-4.mx-auto.text-center(class='md:w-4/12')
        p.mt-2.text-sm.text-gray-500
          | Photo by 
          a(href='https://unsplash.com/@fkaregan?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText') Samuel Regan-Asante 
          | on 
          a(href='https://unsplash.com/?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText') Unsplash
        p.mt-2.text-sm.text-gray-500 Lausanne 🇨🇭
        .text-sm.text-blueGray-500.font-semibold.py-1
          | &copy; 
          span#get-current-year 2021 The Doughnut🌍Meter
</template>

<script>
export default {
  name: 'navBar',
  components: {},
};
</script>

<style scoped></style>
