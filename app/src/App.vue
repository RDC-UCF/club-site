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
    <div class="flex-1 flex-row relative hidden bg-main-text-color md:block">
      <KnightOne />
      <KnightTwo />
    </div>
    <div class="flex-1 flex-row relative hidden bg-main-text-color md:block">
      <AboutOne />
      <AboutTwo />
    </div>
  </div>
</template>