<template>
  <div>
      <div class="bg-gradient-to-b p-[2rem] shadow-md shadow-orange-300 from-orange-600 via-orange-500 to-orange-400">
         <div class="max-w-md mx-auto">
            <h1 class="text-white font-bold text-center text-3xl font-signika">Our blessed client said this about us😍</h1>
         </div>
         <div class="grid grid-cols-1 md:grid-cols-2 gap-6 px-[1rem] md:px-[6rem] mt-[3rem]">
             <div class="flex flex-col" v-for="i in testimonies" :key="i">
                 <div class="relative bg-white rounded-xl py-4">
                     <h1 class="font-signika text-orange-600 text-center font-bold">{{ i.title }}</h1>
                     <div class="md:px-[3rem] px-[1rem] text-center py-3">
                     <p>{{ i.testimony }}</p>
                     </div>
                     <div class="bg-white md:right-64 right-[8rem] rotate-45 h-[1.5rem] w-[1.5rem] absolute"></div>
                 </div>
                 <div>
                     <div class="flex justify-center mt-6 items-center space-x-">
                         <div>
                             <img src="../assets/icons/man.png" class="rounded-full h-[3rem] object-cover w-[3rem]" alt="">
                         </div>
                         <div class="leading-tight ml-3">
                             <h1 class="text-white font-signika font-bold">{{ i.testifiedBy }}</h1>
                             <p class="text-slate-100 text-sm">{{i.company}}</p>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
      </div>
  </div>
</template>

<script setup>
import {reactive} from 'vue'
const testimonies = reactive([
    {
        title: '"Incredible Experience"', 
        testimony: 'We had incredble experience working with Mixland and were inpressed they made such a big difference in only three weeks. Our team is so gratefull for wonderful improvements they made and their ability to get familiar with the concept so quickly',
        testifiedBy: 'Wande warren',
        company: 'Ceo ABC Coporation'
    },
    {
        title: '"Dependable Responsive Profesional"', 
        testimony: 'We had incredble experience working with Mixland and were inpressed they made such a big difference in only three weeks. Our team is so gratefull for wonderful improvements they made and their ability to get familiar with the concept so quickly',
        testifiedBy: 'Esther Howard',
        company: 'Ceo Fintech Coporation'
    },
])

</script>

<style>

</style>