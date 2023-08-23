<script setup>
import MyPlans from './components/MyPlans.vue';
const packages = [
  {
    title:"Starter",
    about:"Best option for personal use & for your next project.",
    price:29,
    uses:[
      "Individual configuration",
      "No setup, or hidden fees",
      "Team size: 1 developer",
      "Premium support: 12 months",   
      "Free updates: 12 months"   
    ]

  },
  {
    title:"Company",
    about:"Relevant for multiple users, extended & premium support.",
    price:99,
    uses:[
      "Individual configuration",
      "No setup, or hidden fees",
      "Team size: 10 developers",
      "Premium support: 24 months",
      "Free updates: 24 months"
    ]
  },
  {
    title:"Enterprise",
    about:"Best for large scale uses and extended redistribution rights.",
    price:499,
    uses:[
      "Individual configuration",
      "No setup, or hidden fees",
      "Team size: 100+ developers",
      "Premium support: 36 months",
      "Free updates: 36 months"
    ]
  }
]
</script>

<template>
  <section class="mx-auto ">
    <section class="bg-white dark:bg-gray-900">
      <div class="py-8 px-4 mx-auto max-w-screen-xl lg:py-16 lg:px-6">
        <div class="mx-auto max-w-screen-md text-center mb-8 lg:mb-12">
          <h2 class="mb-4 text-4xl tracking-tight font-extrabold text-gray-900 dark:text-white">Designed for business teams like yours</h2>
          <p class="mb-5 font-light text-gray-500 sm:text-xl dark:text-gray-400">Here at Flowbite we focus on markets where technology, innovation, and capital can unlock long-term value and drive economic growth.</p>
        </div>
        <div class="space-y-8 lg:grid lg:grid-cols-3 sm:gap-6 xl:gap-10 lg:space-y-0">
          <!-- Pricing Card -->
          <MyPlans :plans="packages"/>
        </div>
      </div>
    </section>
  </section>
</template>

<style scoped>

</style>
