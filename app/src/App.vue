<script setup lang="ts">
// import HelloWorld from "./components/HelloWorld.vue";
import Nav from "./components/Nav.vue";
import "./style.css";
import KnightOne from "./components/KnightOne.vue";
import KnightTwo from "./components/KnightTwo.vue";
import AboutOne from "./components/AboutOne.vue";
import AboutTwo from "./components/AboutTwo.vue";
</script>

<template>
  <!-- <div class="mx-[5%] md:mx-[5%] lg:mx-[5%] min-h-screen flex flex-col"> -->
  <div class="mx-[5%] min-h-screen flex flex-col">
    <Nav />
    <Title />
    <div class="flex-1 flex-row relative hidden bg-main-text-color md:block">
      <KnightOne />
      <KnightTwo />
    </div>
    <div class="flex-1 flex-row relative hidden bg-main-text-color md:block">
      <AboutOne />
      <AboutTwo />
    </div>
  </div>
  <!-- <HelloWorld msg="Vite + Vue" /> -->
</template>

<!-- <style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style> -->
