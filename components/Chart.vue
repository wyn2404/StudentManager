<template>
  <v-card width="400" class="mt-10">
    <v-card-title
      >Chart
      <v-divider></v-divider>
    </v-card-title>
    <div>
      <Bar :data="chartData" :options="chartOptions" />
    </div>
  </v-card>
</template>
<script lang="ts" setup>
import { Bar } from "vue-chartjs";

const chartData = ref({
  labels: ["T1", "T2", "T3", "T4", "T5", "T6", "T7", "T8", "T9"],
  datasets: [
    {
      label: "Point",
      backgroundColor: "#9ADE7B",
      data: [7, 2, 6, 9, 10, 10, 9, 7, 10],
    },
  ],
});
const chartOptions = ref({
  responsive: true,
  maintainAspectRatio: false,
});
</script>
