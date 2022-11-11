<template>
  <div
    w="[688.64px]"
    mx="auto"
    my="4"
    flex="~ flex"
    justify="center"
    items="center"
    text="7xl [#FC4F24]"
    font="bold"
    leading="[88px]"
    gap="2"
    class="ux-copywrite"
  >
    <div class="">
      <div
        w="[278px]"
        h="[73px]"
        flex="~ flex"
        justify="around"
        items="center"
        border="~ border 3 black"
        rounded="md"
        rotate="[4deg]"
        class="transformed-box"
      >
        <i class="i-ic-outline-circle text-black w-5" />
        <div class="flex flex-col">
          <span
            class="no-italic font-semibold text-base text-black font-switzer"
          >
            UX Copywrite
          </span>
          <div class="flex items-center justify-between">
            <span class="font-normal text-xs text-[#000000a3] font-switzer">
              Task • 0 of 7 •
            </span>
            <span
              class="flex font-normal text-[#975BEC] items-center text-xs ml-2 font-switzer"
            >
              <i class="i-uil-calender" /> Today
            </span>
          </div>
        </div>
        <!-- <IconTeamIcon /> -->
        <IconTeam />
      </div>
      <div class="normal-box absolute"></div>
    </div>
    <span>Productivity</span>
  </div>
</template>

<style scoped lang="scss">
.ux-copywrite .transformed-box {
  background: linear-gradient(93.43deg, #ffffff -1.04%, #ffffff 101.54%);
  /* span {
      font-family: $switzer;
    } */
}
.ux-copywrite .normal-box {
  width: 257px;
  height: 73px;
  z-index: -1;
  background: #000000;
  border-radius: 4px;
  transform: translate(10px, -60px);
}
</style>
