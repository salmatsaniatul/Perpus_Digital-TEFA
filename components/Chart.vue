<script setup lang="ts">
import Chart from "chart.js/auto";

const labels = ["Januari", "Februari", "Maret", "April", "Mei", "Juni"];

const data = {
  labels: labels,
  datasets: [
    {
      label: "Statistik pengunjung",
      backgroundColor: "rgb(143, 138, 138)",
      bordercolor: "rgba(153, 102, 255, 1)",
      data: [15, 32, 42, 27, 27, 32, 80],
    },
  ],
};
const config = {
  type: "bar",
  data: data,
  options: {},
};

onMounted(() => {
  const myChart = new Chart(document.getElementById("myChart"), config);
});
</script>

<template>
  <div>
    <canvas id="myChart"></canvas>
  </div>
</template>
