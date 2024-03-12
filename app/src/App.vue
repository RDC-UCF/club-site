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
    <div class="flex-1 flex flex-row items-center justify-center p-8 text-center md:text-left">
      <div class="flex-1">
        <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold my-4 text-gray-800">
          Roblox<br> Development<br> Club at UCF.
        </h1>
      </div>
      <div class="flex-1">
        <KnightOne/>
      </div>
    </div>
    <div class="flex-1 flex flex-row relative hidden md:flex">
      <KnightTwo />
    </div>
    <div class="flex-1 flex flex-row relative hidden md:flex">
      <AboutOne />
      <AboutTwo />
    </div>
  </div>
</template>