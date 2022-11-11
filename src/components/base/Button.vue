<script setup lang="ts">
const props = defineProps<{
  shadow: string;
  btnBorder: string;
  bgColor: string;
  color: string;
  label: string;
  icon?: string;
  iconSize?: string;
  iconColor?: string;
  gap?: string;
}>();

// console.log(computedGap.value);
</script>

<template>
  <button
    border="rounded-full"
    w="full"
    font="bold normal"
    text="lg"
    flex="~ flex"
    justify="center"
    items="center"
    h="12"
    :gap="[props.gap?.slice(3)]"
    class="font-public-sans text-lg btn-style"
  >
    <slot class="icon">
      <i v-if="props?.icon" :class="props?.icon" />
    </slot>
    {{ props.label }}
  </button>
</template>

<style lang="scss" scoped>
.btn-style {
  box-shadow: v-bind('props.shadow');
  border: v-bind('props.btnBorder');
  background-color: v-bind('props.bgColor');
  color: v-bind('props.color');
}
.icon {
  width: v-bind('props.iconSize');
  height: v-bind('props.iconSize');
  color: v-bind('props.iconColor');
}
</style>
