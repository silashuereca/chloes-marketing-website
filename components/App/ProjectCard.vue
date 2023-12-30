<template>
  <div>
    <h3 class="text-sm font-medium" v-text="project.name" />
    <p class="text-sm text-gray-600 w-full dark:text-gray-400" v-text="project.description" />
  </div>
</template>

<script setup>
defineProps({
  project: {
    type: Object,
    required: true,
  },
});
</script>
