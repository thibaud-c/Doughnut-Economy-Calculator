<template lang="pug">
#Doughnut-Home.flex.bg-white.h-auto
  .flex.items-center.text-center.px-8(class='lg:text-left md:px-12 lg:w-1/2')
    div
      h2.text-3xl.font-semibold.text-gray-800(class='md:text-4xl')
        | Let us model your 
        span.text-indigo-600 personalized 
        span doughnut
      p.mt-2.text-sm.text-gray-500(class='md:text-base')
        | Our incredible planet already took a big hit because of our greedy behavior. We tend to forget that there is no planet B. We should give our best from today to meet the sustainable development goals. Take a first step now to automatically calculate a doughnut model related to your local economy!
      p.mt-2.text-sm.text-gray-500.font-semibold(class='md:text-base')
        | Coming soon :)
      .flex.justify-center.mt-6(class='lg:justify-start')
        .bg-white.rounded-lg
          .flex.flex-wrap.justify-between(class='md:flex-row')
            form(@submit.prevent="saveEmail")
              button.ease-in-out.px-4.py-3.bg-gray-900.text-gray-200.text-xs.font-semibold.rounded.shadow-2xl(type="submit" class='hover:bg-gray-800 transition-duration: 150ms' :disabled="isEmailSubmitted") {{notifyBtnLabel}}
              input.ease-in-out.m-3.p-2.appearance-none.text-gray-700.text-sm.border.rounded-lg(v-if="!isEmailSubmitted" type='email', id="email", required, pattern="^[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,4}$", class='focus:outline-none transition-duration: 250ms', placeholder='you@somewhere.com', v-model="userEmail")
  .hidden(class='lg:block lg:w-1/2', style='clip-path:polygon(10% 0, 100% 0%, 100% 100%, 0 100%)')
    img.w-full.object-cover.object-center.shadow-xl(style="heigh:600px", src="../assets/images/doughnut_time.jpg")
</template>

<script>
import { ref } from 'vue';
import firebaseDB from '../utils/firebase';
import { getDatabase, ref as firebase_ref, set } from "firebase/database";

export default {
  name: 'introBanner',
  components: {},
  setup() {
    let userEmail = ref('');
    let notifyBtnLabel = ref('Notify Me On Launch');
    let isEmailSubmitted = ref(false)

    const uuidv4 = () => {
      return 'xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx'.replace(/[xy]/g, function(c) {
        var r = Math.random() * 16 | 0, v = c == 'x' ? r : (r & 0x3 | 0x8);
        return v.toString(16);
      });
    }
    const updateEmailState = () => {
      userEmail.value = ''
      notifyBtnLabel.value = 'Thank you ❤️'
      isEmailSubmitted.value = true
    }

    const saveEmail = () => {
      const db = getDatabase(firebaseDB);
      set(firebase_ref(db, 'emails/' + uuidv4()), {
        "timestamp": (new Date()).getTime(),
        "email":userEmail.value
      })
      updateEmailState();
    }
  
    return { userEmail, saveEmail, notifyBtnLabel, isEmailSubmitted };
  }
};
</script>

<style scoped></style>
