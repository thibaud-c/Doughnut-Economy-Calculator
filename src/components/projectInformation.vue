<template lang="pug">
#The-Doughnut-Project.h-auto
  .flex.bg-white.py-4
    .hidden(class='lg:block lg:w-1/2')
    .flex.items-center.px-8(class='lg:left-right md:px-12 lg:w-1/3')
      div
        h2.text-3xl.font-semibold.text-gray-800(class='md:text-4xl')
          | What is the 
          span.text-indigo-600 doughnut
          span (🌍meter) economy?
        p.mt-2.text-sm.text-gray-500(class='md:text-base')
          | Mentioned first in Kate Raworth’s paper ˝A safe and just space for humanity˝, doughnut economic model is a concept of sustainable development whose main goals are to bring social foundations to every person, but not to burden the planet in the process and exploit the nature to the point of no return. The economy throughout the world for now is based on growth, but this growth can’t go on forever since we have limited resources on the planet. It’s time to bring a change and make the world safer and more equal between the countries. 
  .flex.bg-white.py-4
    .flex.items-center.px-8(class='lg:text-left md:px-12 lg:w-1/3')
      div
        h2.text-3xl.font-semibold.text-gray-800(class='md:text-4xl')
          | How do we  
          span.text-indigo-600 calculate 
          span the doughnut model?
        p.mt-2.text-sm.text-gray-500(class='md:text-base')
          | The first step of implementing a doughnut economy is to establish the current situation in a specific country/city. We do this by getting information about every indicator of social foundations (e.g. food, education, health, income and work…), and also the ecological ceiling indicators (e.g. climate change, biodiversity loss, ozone layer depletion…). This allows us to visualize the doughnut – to see where the country stands and what are the factors that need most immediate action. 
    .hidden(class='lg:block lg:w-1/2')
  .flex.bg-white.py-4
    .hidden(class='lg:block lg:w-1/2')
    .flex.items-center.px-8(class='lg:text-left md:px-12 lg:w-1/3')
      div
        h2.text-3xl.font-semibold.text-gray-800(class='md:text-4xl')
          | Why does the 
          span.text-indigo-600 doughnut🌍meter 
          span matter?
        p.mt-2.text-sm.text-gray-500(class='md:text-base')
          | The greedy nature of people in charge all around the world is directly influencing the natural resources that are already very limited. In order to continue living like we do now, we would need 5 planets as natural resources. Since we only have one, we have to change the approach and implement a sustainable, doughnut economy in the place of never ending and impossible growth.
</template>

<script>
import { ref } from 'vue';

export default {
  name: 'introBanner',
  components: {},
  setup() {}

};
</script>

<style scoped></style>
