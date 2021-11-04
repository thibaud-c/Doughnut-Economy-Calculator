<template lang="pug">
#Team-o-Doughnut.flex.flex-wrap.bg-white.h-auto
  .flex.items-center.text-center.px-8.py-4(class='lg:text-left md:px-12 lg:w-1/2')
    div
      h2.text-3xl.font-semibold.text-gray-800(class='md:text-4xl')
        | Our doughnut 
        span.text-indigo-600 family
        span . Let's keep in touch!
      p.mt-2.text-sm.text-gray-500(class='md:text-base') We are building this project 🍩-by-🍩 because we believe that sustainable development is crutial for our planet. If you share our vision don't hesitate to show us your support by  
        a.mt-2.text-sm.text-indigo-600(class='md:text-base' href='https://www.buymeacoffee.com/doughnutometer') offering us a small 🍩 
  .flex(class='md:px-12 lg:w-1/2')
    .grid.gap-4.auto-cols-auto(class='sm:grid-cols-1 md:grid-cols-2 xl:grid-cols-2')
      .flex.flex-col.items-center.justify-center.bg-white.p-4.shadow.rounded-lg.w-full
        .inline-flex.shadow-lg.border.border-gray-200.rounded-full.overflow-hidden.h-40.w-40
          img.h-full.w-full(src='https://media2.giphy.com/media/4Iw2OzgiiTc4M/giphy.webp?cid=ecf05e47h8ldevjulbgav55fbdo108bd6c9ounh2hm1qtfl3&rid=giphy.webp&ct=g', alt='')
        h2.mt-4.font-bold.text-xl Milica Mihailovic
        h6.mt-2.text-sm.font-medium #Brain #Girlfriend
        p.text-xs.text-gray-500.text-left.font-semibold.mt-3
          | Favorite doughnut flavor: 
          span.text-xs.text-gray-500.text-left.mt-3.font-normal Vanilla filling, nutella topping
        ul.flex.flex-row.mt-4.space-x-2
          li
            a.text-gray-500(href='https://www.linkedin.com/in/milica-mihailovic-862671192/', class='hover:text-gray-600')
              svg.w-6.h-6(aria-hidden='true', fill='currentColor', viewbox='0 0 24 24')
                path(fill-rule='evenodd', d='M4.98 3.5c0 1.381-1.11 2.5-2.48 2.5s-2.48-1.119-2.48-2.5c0-1.38 1.11-2.5 2.48-2.5s2.48 1.12 2.48 2.5zm.02 4.5h-5v16h5v-16zm7.982 0h-4.968v16h4.969v-8.399c0-4.67 6.029-5.052 6.029 0v8.399h4.988v-10.131c0-7.88-8.922-7.593-11.018-3.714v-2.155z', clip-rule='evenodd')
          li
            a.text-gray-500(href='mailto:mmihailovic97@gmail.com', class='hover:text-gray-600')
              svg.w-6.h-6(aria-hidden='true', fill='currentColor', viewbox='0 0 24 24')
                path(fill-rule='evenodd', d='M12.042 23.648c-7.813 0-12.042-4.876-12.042-11.171 0-6.727 4.762-12.125 13.276-12.125 6.214 0 10.724 4.038 10.724 9.601 0 8.712-10.33 11.012-9.812 6.042-.71 1.108-1.854 2.354-4.053 2.354-2.516 0-4.08-1.842-4.08-4.807 0-4.444 2.921-8.199 6.379-8.199 1.659 0 2.8.876 3.277 2.221l.464-1.632h2.338c-.244.832-2.321 8.527-2.321 8.527-.648 2.666 1.35 2.713 3.122 1.297 3.329-2.58 3.501-9.327-.998-12.141-4.821-2.891-15.795-1.102-15.795 8.693 0 5.611 3.95 9.381 9.829 9.381 3.436 0 5.542-.93 7.295-1.948l1.177 1.698c-1.711.966-4.461 2.209-8.78 2.209zm-2.344-14.305c-.715 1.34-1.177 3.076-1.177 4.424 0 3.61 3.522 3.633 5.252.239.712-1.394 1.171-3.171 1.171-4.529 0-2.917-3.495-3.434-5.246-.134z', clip-rule='evenodd')
      .flex.flex-col.items-center.justify-center.bg-white.p-4.shadow.rounded-lg.w-full
        .inline-flex.shadow-lg.border.border-gray-200.rounded-full.overflow-hidden.h-40.w-40
          img.h-full.w-full(src='https://media0.giphy.com/media/n8h4ZcU02Vg25ct7e6/giphy.webp', alt='')
        h2.mt-4.font-bold.text-xl Thibaud Chassin
        h6.mt-2.text-sm.font-medium #Geek #Boyfriend
        p.text-xs.text-gray-500.text-left.font-semibold.mt-3
          | Favorite doughnut flavor: 
          span.text-xs.text-gray-500.text-left.mt-3.font-normal Chocolate filling, hazelnut crumb topping
        ul.flex.flex-row.mt-4.space-x-2
          li
            a.text-gray-500(href='https://www.linkedin.com/in/thibaud-chassin/', class='hover:text-gray-600')
              svg.w-6.h-6(aria-hidden='true', fill='currentColor', viewbox='0 0 24 24')
                path(fill-rule='evenodd', d='M4.98 3.5c0 1.381-1.11 2.5-2.48 2.5s-2.48-1.119-2.48-2.5c0-1.38 1.11-2.5 2.48-2.5s2.48 1.12 2.48 2.5zm.02 4.5h-5v16h5v-16zm7.982 0h-4.968v16h4.969v-8.399c0-4.67 6.029-5.052 6.029 0v8.399h4.988v-10.131c0-7.88-8.922-7.593-11.018-3.714v-2.155z', clip-rule='evenodd')

          li
            a.text-gray-500(href='mailto:thibaud.chassin@gmail.com', class='hover:text-gray-600')
              svg.w-6.h-6(aria-hidden='true', fill='currentColor', viewbox='0 0 24 24')
                path(fill-rule='evenodd', d='M12.042 23.648c-7.813 0-12.042-4.876-12.042-11.171 0-6.727 4.762-12.125 13.276-12.125 6.214 0 10.724 4.038 10.724 9.601 0 8.712-10.33 11.012-9.812 6.042-.71 1.108-1.854 2.354-4.053 2.354-2.516 0-4.08-1.842-4.08-4.807 0-4.444 2.921-8.199 6.379-8.199 1.659 0 2.8.876 3.277 2.221l.464-1.632h2.338c-.244.832-2.321 8.527-2.321 8.527-.648 2.666 1.35 2.713 3.122 1.297 3.329-2.58 3.501-9.327-.998-12.141-4.821-2.891-15.795-1.102-15.795 8.693 0 5.611 3.95 9.381 9.829 9.381 3.436 0 5.542-.93 7.295-1.948l1.177 1.698c-1.711.966-4.461 2.209-8.78 2.209zm-2.344-14.305c-.715 1.34-1.177 3.076-1.177 4.424 0 3.61 3.522 3.633 5.252.239.712-1.394 1.171-3.171 1.171-4.529 0-2.917-3.495-3.434-5.246-.134z', clip-rule='evenodd')

          li
            a.text-gray-500(href='https://github.com/thibaud-c', class='hover:text-gray-600')
              svg.w-6.h-6(aria-hidden='true', fill='currentColor', viewbox='0 0 24 24')
                path(fill-rule='evenodd', d='M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z', clip-rule='evenodd')
</template>

<script>
export default {
  name: 'navBar',
  components: {},
};
</script>

<style scoped></style>
