<template>
  <Header />
  <main class="flex justify-center items-center mt-20 flex-col">
    <v-card width="400">
      <div class="flex justify-between p-4">
        <v-avatar>
          <v-img src="https://cdn.vuetifyjs.com/images/john.jpg" alt="John" />
        </v-avatar>
        <span class="ml-3 text-black">Huynh Quy</span>
        <span class="ml-3 font-medium text-sky-500">11B5</span>
      </div>
    </v-card>
    <Extension />
    <Chart />
    <New />
  </main>
</template>
<style>
</style>
