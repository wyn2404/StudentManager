<template>
  <header
    class="bg-white w-full flex justify-between h-14 items-center fixed z-50 top-0 shadows"
  >
    <v-app-bar-nav-icon></v-app-bar-nav-icon>
    <div class="mobile">
      <v-btn variant="text">Exam</v-btn>
      <v-btn variant="text">Information</v-btn>
      <v-btn variant="text">Setting</v-btn>
      <v-btn variant="text">About</v-btn>
      <span v-if="colorMode.value === 'dark'">Hello</span>
      <span class="dark:bg-sky-700">hello</span>
    </div>
    <div>
      <v-btn icon variant="text" @click="OnClick">
        <v-icon>mdi-white-balance-sunny</v-icon>
      </v-btn>
      <v-btn icon variant="text">
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>
    </div>
  </header>
</template>
<script setup lang="ts">
const colorMode = useColorMode();
const OnClick = () => (colorMode.preference = (colorMode.value === 'light' ? 'dark' : 'light'), console.log(colorMode.value))

</script>
<style>
@media screen and (max-width: 768px) {
  .mobile {
    display: none;
  }
}
.text-sky-500 {
  --tw-text-opacity: 1;
  color: rgb(14 165 233 / var(--tw-text-opacity));
}
.shadows {
  box-shadow: 0px 2px 1px -1px var(--v-shadow-key-umbra-opacity, rgba(0, 0, 0, 0.2)),
    0px 1px 1px 0px var(--v-shadow-key-penumbra-opacity, rgba(0, 0, 0, 0.14)),
    0px 1px 3px 0px var(--v-shadow-key-penumbra-opacity, rgba(0, 0, 0, 0.12));
}
</style>
