<template>
  <div>
    <h2 class="uppercase text-xs font-semibold text-gray-400 mb-6">
      FEATURED PROEJCTS
    </h2>
    <div class="space-y-4">
      <AppProjectCard
        v-for="(project, id) in projects"
        :key="id"
        :project="project"
      />
    </div>
  </div>
</template>

<script lang="ts" setup>
const { data: projects } = await useAsyncData("projects-home", () => {
  const data = queryContent("/projects").find();
  return data;
});
</script>
