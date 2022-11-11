<template>
  <main>
    <VSpacer space="my-[150px]" />
    <Hero />
  </main>
</template>

<script setup lang="ts">
import { useHead } from '@vueuse/head';

const siteData = reactive({
  title: `Finstack - Plan your project`,
  description: `Plan projects, stay on track, and deliver on time without overworking your team.`,
});

useHead({
  // Can be static or computed
  title: () => siteData.title,
  meta: [
    {
      name: `description`,
      content: () => siteData.description,
    },
  ],
});
</script>

<style lang="scss" scoped></style>
