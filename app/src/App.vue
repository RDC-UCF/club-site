<script setup lang="ts">
import Nav from "./components/Nav.vue";
import "./style.css";
import KnightOne from "./components/KnightOne.vue";
import KnightTwo from "./components/KnightTwo.vue";
import AboutOne from "./components/AboutOne.vue";
import AboutTwo from "./components/AboutTwo.vue";
</script>

<template>
  <div class="min-h-screen flex flex-col bg-gradient-to-t from-[#B5A26A] to-[#F8FAFC]">
    <Nav />
    <div class="flex-1 px-4 md:px-8 lg:px-16 xl:px-32" style="padding-top: var(--navbar-height);">
      <div class="flex flex-col md:flex-row items-center justify-between text-center md:text-left h-full">
        <h1 class="text-3xl md:text-4xl lg:text-5xl xl:text-6xl font-bold my-4 text-gray-800 flex-1">
          Roblox<br> Development<br> Club at UCF.
        </h1>
        <div class="flex-1">
          <KnightOne class="w-full h-auto"/>
        </div>
      </div>
    </div>
    <div class="flex-1 hidden md:flex">
      <KnightTwo />
    </div>
    <div class="flex-1 hidden md:flex">
      <AboutOne />
      <AboutTwo />
    </div>
  </div>
</template>

<style>
:root {
  --navbar-height: 64px;
}
</style>