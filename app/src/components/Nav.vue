<template>
  <div class="fixed top-0 left-0 w-full z-10">
    <nav :class="{ 'translate-y-0': isShown, '-translate-y-full': !isShown, 'opacity-100': isShown, 'opacity-0': !isShown }" class="transform transition-opacity duration-300 w-full">
      <div class="flex justify-between items-center w-full p-4">
        <a href="/" class="flex items-center">
          <img src="/logo1.png" alt="RDC @ UCF" class="h-8">
          <span class="flex items-center space-x-4 justify-end">RDC @ UCF</span>
        </a>
        <div class="flex items-center space-x-4 justify-end">
          <a href="/about" class="hover:text-gray-700">About</a>
          <a href="/our-team" class="hover:text-gray-700">Our Team</a>
          <a href="/calendar" class="hover:text-gray-700">Calendar</a>
          <a href="/contact" class="hover:text-gray-700">Contact Us</a>
          <a href="https://discord.gg/ASngpDyJGg" target="_blank" rel="noopener noreferrer">
            <img src="/discord_logo.png" alt="Discord" class="h-6">
          </a>
        </div>
      </div>
    </nav>
  </div>
</template>

<script lang="ts">
import { ref, onMounted, onUnmounted } from 'vue';

export default {
  setup() {
    const isShown = ref(true);

    const handleScroll = () => {
      const currentScrollPosition = window.pageYOffset;
      isShown.value = currentScrollPosition <= 0;
    };

    onMounted(() => {
      window.addEventListener('scroll', handleScroll);
    });

    onUnmounted(() => {
      window.removeEventListener('scroll', handleScroll);
    });

    return { isShown };
  }
};
</script>

<style scoped>
nav {
  font: 550 16px/24px 'Inter Semi-Bold', sans-serif;
  transition: opacity 1.5s ease-in-out, 
  transform 1.5s ease-in-out;
}
</style>
