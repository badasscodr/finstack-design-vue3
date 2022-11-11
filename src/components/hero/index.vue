<script setup lang="ts">
// import { IconInlineTeam, IconTeamIcon } from '../icons';
</script>

<template>
  <section class="border w-full hero">
    <div>
      <h1
        flex="~ flex"
        w="[770px]"
        mx="auto"
        justify="center"
        text="7xl"
        items="center"
        font="bold"
        leading="[88px]"
      >
        Manage You <IconInlineTeam /> Team's
      </h1>
      <HeroSubhead />
      <VSpacer space="my-12" />
      <p
        class="mx-auto w-[499px] font-switzer font-medium text-xl text-center color-[#000000b8]"
      >
        Plan projects, stay on track, and deliver on time without overworking
        your team.
      </p>
      <VSpacer space="my-12" />
      <HeroBtn />
      <VSpacer space="my-10" />
      <div class="flex justify-center items-center gap-2">
        <i class="i-material-symbols-check-circle text-base text-[#333333]" />
        <span class="font-switzer font-normal text-base"
          >Excellent 4.9 out of 5</span
        >
        <img src="@/assets/img/hero-rating-img.png" w="20" h="6" alt="" />
      </div>
    </div>
  </section>
  <HeroSticky />
</template>

<style lang="scss" scoped></style>
