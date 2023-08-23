<script setup>``
import BlogPost from './components/BlogPost.vue';

const posts=[
  {
    title: "Deadbeef Decrementation",
    excerpt: "How to decrement from a magic debug value to zero.",
    tags: "spirituality",
    date: "2016-10-09",
    linkColor:"#6366F1"
  },
  {
    title: "Interior Crocodile Alligator, I Drive a Chevrolet Movie Theater",
    excerpt: "♫ Interior Crocodile Alligator, I Drive a Chevrolet Movie Theater ♫",
    tags: "cats",
    date: "2008-09-19",
    linkColor:"#F59E0B"
  },
  {
    title: "Why My Practice of Thelema Makes Me Better at World of Warcraft",
    excerpt: "\"Do what thou wilt\" shall be the whole of the Law.",
    tags: "enchiladas",
    date: "1974-09-09",
    linkColor:"#10B981"
  },
  {
    title:'Shrek Predicted the COVID-19 Pandemic',
    excerpt:'Find out how Shrek is disrupting astrology.',
    tags:"orcas",
    date:'1921-04-16',
    linkColor:"#EF4444",
  },
  {
    title:'Lorem Ipsum',
    excerpt:'You know what time it is: lorem ipsum time.',
    tags:'stoicism',
    date:'1918-11-04',
    linkColor:"#8B5CF6"
  }
]
</script>

<template>
  <section class="mx-auto ">
    <header>
      <nav class="container mx-auto max-w-3xl px-8 pt-2 flex flex-wrap justify-between">
        <div>
          <h1>
            <a href="/11r/">11r</a>
          </h1>
          <p>america's favorite eleventy blog template</p>
        </div>

        <ul class="flex flex-wrap sm:w-32 w-full mt-6 md:justify-between justify-evenly">
          <li>
            <a href="/11r/404.html">404</a>
          </li>

          <li>
            <a href="/11r/about">About</a>
          </li>
        </ul>
      </nav>
    </header>
    <main class="container mx-auto max-w-3xl p-8 grow">

      <div>


        <BlogPost :BlogPosts="posts" />

        <p class="text-center text-sm italic mb-10">(On page
          1
          of
          2.)</p>
      </div>

      <div class="grid grid-flow-row grid-cols-3 gap-4 mb-2">
        <a class="tag cats mx-auto" href="/11r/tag/cats">cats</a>
        <a class="tag enchiladas mx-auto" href="/11r/tag/enchiladas">enchiladas</a>
        <a class="tag beer mx-auto" href="/11r/tag/beer">beer</a>
        <a class="tag spirituality mx-auto" href="/11r/tag/spirituality">spirituality</a>
        <a class="tag orcas mx-auto" href="/11r/tag/orcas">orcas</a>
        <a class="tag stoicism mx-auto" href="/11r/tag/stoicism">stoicism</a>
      </div>


    </main>
  </section>
</template>

<style scoped>

</style>
