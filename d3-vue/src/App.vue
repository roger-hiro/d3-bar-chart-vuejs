<template>
  <div id="app">
    <BarChart title="Bar Chart" xKey="name" yKey="amount" :data="barChartData"/>
  </div>
</template>

<script>
import BarChart from "./components/BarChart.vue";

export default {
  name: "App",
  components: {
    BarChart
  },
  data: () => ({
    barChartData: [
      {
        name: "Roses",
        amount: 25
      },
      {
        name: "Tulips",
        amount: 40
      },
      {
        name: "Daisies",
        amount: 15
      },
      {
        name: "Narcissuses",
        amount: 9
      }
    ]
  })
};
</script>

<style>
#app {
  font-family: "Open Sans", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #282f36;
  margin-top: 30px;
}
</style>
