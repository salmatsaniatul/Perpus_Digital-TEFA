<script setup lang="ts">
import Chart from 'chart.js/auto';

const labels = ['Januari', 'Februari', 'Maret', 'April', 'Mei', 'Juni'];

const data = {
  labels: labels,
  datasets: [
    {
      label: 'My First Datasets',
      backgroundcolor: 'black',
      bordercolor: 'while',
      data: [0, 10, 15, 2, 20, 30, 45],
    },
  ],
};
const config = {
  type: 'bar',
  data: data,
  options: {},
};

onMounted(() => {
  const myChart = new Chart(document.getElementById('myChart'), config);
});
</script>
<template>
  <div>
    <canvas id="myChart"></canvas>
  </div>
</template>

<style scoped>
.backgroundcolor {
  background-color: #8f8a8a !important;
}
</style>
