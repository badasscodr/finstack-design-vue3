<script setup lang="ts">
const props = defineProps<{ space: string }>();
</script>

<template>
  <div :class="props.space" />
</template>
