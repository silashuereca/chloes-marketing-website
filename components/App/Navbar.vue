<template>
  <div ref="headerRef" :style="styles" class="fixed top-0 w-full z-50">
    <nav class="mx-auto px-4 sm:px-6 lg:px-8 max-w-2xl">
      <ul
        class="flex items-center my-4 px-3 text-sm font-medium text-gray-800 rounded-full shadow-lg bg-white/90 shadow-gray-800/5 ring-1 backdrop-blur dark:bg-gray-800/90 dark:text-gray-200 dark:ring-white/20 ring-gray-900/5"
      >
        <li class="py-4">
          <NuxtLink to="/">
            Home
          </NuxtLink>
        </li>
        <li class="ml-3 py-4">
          <NuxtLink to="#stay-in-touch">
            Contact
          </NuxtLink>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script setup>
import { useFixedHeader } from 'vue-use-fixed-header'
const headerRef = ref(null);
const { styles } = useFixedHeader(headerRef);
</script>

<style>
html {
  scroll-behavior: smooth;
}
</style>