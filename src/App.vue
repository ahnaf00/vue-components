<script setup>
import TodoList from './components/TodoList.vue';
const Frodo = [
  {title: 'Weed front garden.',             completed: true},
  {title: 'Chill and smoke some Old Toby.', completed: true},
  {title: 'Keep ring secret and safe.',     completed: false},
  {title: 'Meet Gandalf at Bree.',          completed: false},
  {title: 'Destroy ring and defeat dark lord.', completed: false},
]

const Sam = [
  {title: 'Trim the verge.',                completed: true},
  {title: 'Eavesdrop on Master Frodo & Gandalf.', completed: true},
  {title: 'Boil, mash, and stick potatoes in stew.', completed: false},
  {title: 'Carry Frodo.',                   completed: false},
  {title: 'Be all round legend.',           completed: false},
]
</script>

<template>
  <section class="mx-auto ">
    <h1 class="my-10 text-center">Components</h1>
    <div class="flex items-center justify-center h-[600px] font-medium">
      <div class="flex flex-grow items-center justify-center h-full text-gray-600 bg-gray-100">
        <!-- Component Start -->
        <TodoList title="Frodo's Jobs" :tasks="Frodo" background="bg-white"/>
        <!-- Component End  -->
      </div>
      <div class="flex flex-grow items-center justify-center bg-gray-900 h-full">
        <!-- Component Start -->
        <TodoList title="Sam's Jobs" :tasks="Sam" background="bg-gray-800"/>
        <!-- Component End  -->

      </div>
    </div>

  </section>
</template>

<style scoped>

</style>
