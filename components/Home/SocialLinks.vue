<template>
  <div>
    <h2 class="uppercase text-xs font-semibold text-gray-400 mb-4">Let's connect</h2>
    <div class="space-y-5">
      <NuxtLink
        v-for="link in links"
        :key="link.icon"
        :to="link.url"
        target="_blank"
        external
        class="flex items-end gap-4 dark:hover:text-gray-300 group"
      >
        <span class="text-sm" v-text="link.name" />
        <div
          class="flex-1 border-b border-dashed border-gray-300 dark:border-gray-800 group-hover:border-gray-700"
        ></div>
        <Icon :name="link.icon" class="w-6 h-6"></Icon>
      </NuxtLink>
    </div>
  </div>
</template>

<script lang="ts" setup>
const links = [
  {
    name: "Linkedin",
    url: "https://www.linkedin.com/in/chloehuereca2015/",
    icon: "mdi:linkedin",
  },
];
</script>
