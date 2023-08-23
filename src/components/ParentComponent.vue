<script setup>

import TeamMember from './TeamMember.vue';

const person1 = {
  name:"Bonnie Green",
  designation:"CEO & Web Developer",
  about:"Bonnie drives the technical strategy of the flowbite platform and brand.",
  image:"//flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/bonnie-green.png",
}
const person2 = {
  name:"Jese Leos",
  designation:"CTO",
  about:"Jese drives the technical strategy of the flowbite platform and brand.",
  image:"//flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/joseph-mcfall.png",
}
const person3 = {
  name:"Michael Gough",
  designation:"Senior Front-end Developer",
  about:"Michael drives the technical strategy of the flowbite platform and brand.",
  image:"//flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/michael-gouch.png",
}
const person4 = {
  name:"Lana Byrd",
  designation:"Marketing & Sal",
  about:"Bonnie drives the technical strategy of the flowbite platform and brand.",
  image:"//flowbite.s3.amazonaws.com/blocks/marketing-ui/avatars/sofia-mcguire.png",
}
</script>


<template>
  <section class="bg-white dark:bg-gray-900">
    <div class="py-8 px-4 mx-auto max-w-screen-xl lg:py-16 lg:px-6 ">
      <div class="mx-auto max-w-screen-sm text-center mb-8 lg:mb-16">
          <h2 class="mb-4 text-4xl tracking-tight font-extrabold text-gray-900 dark:text-white">Our Team</h2>
          <p class="font-light text-gray-500 lg:mb-16 sm:text-xl dark:text-gray-400">Explore the whole collection of open-source web components and elements built with the utility classes from Tailwind</p>
      </div>
      <div class="grid gap-8 mb-6 lg:mb-16 md:grid-cols-2">
          <!-- <TeamMember :name="person1.name" :designation="person1.designation" :about="person1.about" :image="person1.image" /> -->
          <TeamMember v-bind="person1" />
          <TeamMember v-bind="person2" />
          <TeamMember v-bind="person3"/>
          <TeamMember v-bind="person4" />
      </div>
    </div>
  </section>
</template>


<style scoped></style>