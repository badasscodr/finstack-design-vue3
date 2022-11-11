<template>
  <nav
    class="mx-auto my-10 px-12 rounded-3xl w-[1170px] h-24 bg-white grid grid-cols-3 items-center"
  >
    <div class="col-span-2 grid grid-cols-4 items-center">
      <div class="flex items-center space-x-4">
        <img
          src="https://i.ibb.co/17NfBDr/image.png"
          width="40"
          height="40"
          alt=""
        />
        <span
          class="leading-10 not-italic font-bold text-2xl logo-text cursor-default"
        >
          Finstack
        </span>
      </div>
      <div class="col-span-2 flex justify-around">
        <span
          v-for="label in primaryMenu"
          :key="label.id"
          class="cursor-pointer menu-text not-italic font-normal text-lg"
        >
          {{ label.label }}
        </span>
      </div>
    </div>
    <div class="justify-self-end w-32">
      <Button
        shadow="7px 7px 0px #000000"
        btnBorder="3px solid #000000"
        bg-color="#FFFFFF"
        color="#000000"
        label="Join Free"
        icon-color="#FFFFFF"
        icon-size="20"
      />
    </div>
  </nav>
</template>

<style lang="scss" scoped>
nav {
  box-shadow: 0px 8px 100px rgba(0, 0, 0, 0.03);
  .logo-text {
    font-family: $cabinet-grotesk;
  }
  .menu-text {
    font-family: $switzer;
  }
  button {
    box-shadow: 4px 4px 0px #000000;
    font-family: $public-sans;
  }
}
</style>
