<script setup lang="ts">
import Nav from "./components/Nav.vue";
import "./style.css";
import KnightOne from "./components/KnightOne.vue";
import KnightTwo from "./components/KnightTwo.vue";
import AboutOne from "./components/AboutOne.vue";
import AboutTwo from "./components/AboutTwo.vue";
</script>

<template>
  <div class="flex flex-col bg-gradient-to-t from-[#B5A26A] to-[#F8FAFC]">
    <Nav />
    <div class="flex-1 flex flex-col md:flex-row items-center justify-center text-center md:text-left pt-[var(--navbar-height)] px-[2rem] md:px-[4rem] lg:px-[6rem] xl:px-[8rem]" style="min-height: calc(100vh - var(--navbar-height));">
      <h1 class="title text-4xl md:text-6xl lg:text-8xl xl:text-16xl font-bold my-4 text-gray-800">
        Roblox<br> Development<br> Club at UCF.
      </h1>
      <KnightOne class="logo w-[80vw] h-[80vh] md:w-[55vw] md:h-[55vh] lg:w-[80vw] lg:h-[80vh] object-contain mx-auto"/>
    </div>
    <div class="section min-h-screen">
      <KnightTwo />
    </div>
    <div class="section min-h-screen">
      <AboutOne />
      <AboutTwo />
    </div>
  </div>
</template>

<style scoped>
.title {
  transition: font-size 0.3s ease-in-out;
}

.logo {
  transition: width 0.3s ease-in-out, height 0.3s ease-in-out;
}

.section {
  min-height: 100vh;}
</style>