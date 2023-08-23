<script setup>
import CardBody from "./components/CardBody.vue";

const card_1 = {
  title:"The Magnificent Bogra",
  para:"Located in Rajshahi Division, Bogra is one of the oldest and most fascinating towns in Bangladesh",
  img:"https://i.ibb.co/Kr4b0zJ/152013403-10158311889099633-8423107287930246533-o.jpg",
  distanceInfo:"196 km",
  reviews:"16 reviews",
  placesToVisit:"*Places to visit: Mahasthangarh, Vasu Bihar & Momo Inn",
  btnLink:"Book Ticket"
}


</script>

<template>
  <section class="mx-auto ">
    <h1 class="my-5 text-center">Components</h1>
    <div class="flex flex-col space-y-5  text-left">

      <CardBody :cards="card_1"/>

      <CardBody :cards="card_1"/>
    </div>

  </section>
</template>

<style scoped></style>
