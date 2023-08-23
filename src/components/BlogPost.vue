<script setup>
import { reactive } from "vue";
defineProps(["BlogPosts"]);
const customStyle = reactive({
    backgroundColor: "red",
})
</script>

<template>
    <div class="mb-8 border-dotted border-b pb-8 border-gray-300" v-for="(post, index) in BlogPosts" :key="index">
        <h2>
        <a class="block" href="/11r/post/deadbeef-decrementation/">{{ post.title }}</a>
        </h2>

        <p class="excerpt">{{ post.excerpt }}</p>

        <a class="tag spirituality"  :style="{ backgroundColor:post.linkColor }" href="/11r/tag/spirituality">{{ post.tags }}</a>

        <span class="block md:inline md:float-right md:pt-4 pt-2 created-date" datetime="Sat Oct 08 2016 19:00:00 GMT-0500 (Central Daylight Time)">
        {{ post.date }}
        </span>
    </div>
</template>

<style scoped></style>