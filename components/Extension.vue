<template>
  <v-card class="mt-10 absolute z-50" width="400">
    <v-card-title class="">
      <span>Extension</span>
      <v-divider></v-divider>
    </v-card-title>
    <div class="grid grid-cols-2 gap-4 p-7">
      <v-btn color="#557C55" class="text-white">
        Exam
        <v-tooltip activator="parent" location="start">Homework your</v-tooltip>
      </v-btn>
      <v-btn color="#748E63" class="text-white" append-icon="mdi-book">
        Homework
        <v-tooltip activator="parent" location="end">Homework your</v-tooltip>
      </v-btn>
      <v-btn color="#508D69" class="text-white" append-icon="mdi-file-document">
        Documents
        <v-tooltip activator="parent" location="start">Homework your</v-tooltip>
      </v-btn>
      <v-btn color="#739072" class="text-white">
        Tut
        <v-tooltip activator="parent" location="end">Homework your</v-tooltip>
      </v-btn>
    </div>
  </v-card>
</template>
