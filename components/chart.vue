<script setup lang="ts">
import Chart from "chart.js/auto";

const labels = {
  Januari: "Februari",
  Maret: "April",
  Mei: "Juni",
  Juli: "Agustus",
  September: "Oktober",
  November: "Desember",
};

const data = {
  labels: labels,
  datasets: [
    {
      label: "My First Datasets",
      backgroundcolor: "black",
      bordercolor: "while",
      data: [0, 10, 15, 2, 20, 30, 45],
    },
  ],
};
const config = {};
</script>
<template>
  <div>
    <canvas id="myChart"></canvas>
  </div>
</template>
