<script>
export default {
  name: "App",
  data() {
    return {
      series: [
        {
          name: "Hedef",
          color: "#05e836",
          data: [
            {
              x: "Hedef",
              y: 100,
              fillColor: "#05e836",
            },
            {
              x: "Hedef",
              y: 0,
            },
            {
              x: "Hedef",
              y: 0,
            },
          ],
        },
        {
          name: "Faturalandırılmış",
          color: "#6a00ff",
          data: [
            {
              x: "Faturalandırılmış",
              y: 0,
            },
            {
              x: "Faturalandırılmış",
              y: 20,
              fillColor: "#6a00ff",
            },
            {
              x: "Faturalandırılmış",
              y: 0,
            },
          ],
        },
        {
          name: "Faturalandırılmamış",
          color: "#b37dff",
          data: [
            {
              x: "Faturalandırılmamış",
              y: 0,
            },
            {
              x: "Faturalandırılmamış",
              y: 30,
              fillColor: "#b37dff",
            },
            {
              x: "Faturalandırılmamış",
              y: 0,
            },
          ],
        },
        {
          name: "Ilık",
          color: "#d4fff3",
          data: [
            {
              x: "Ilık",
              y: 0,
            },
            {
              x: "Ilık",
              y: 0,
            },
            {
              x: "Ilık",
              y: 10,
              fillColor: "#d4fff3",
            },
          ],
        },
        {
          name: "Sıcak",
          color: "#ff7519",
          data: [
            {
              x: "Sıcak",
              y: 0,
            },
            {
              x: "Sıcak",
              y: 0,
            },
            {
              x: "Sıcak",
              y: 80,
              fillColor: "#ff7519",
            },
          ],
        },
        {
          name: "Soğuk",
          color: "#7accff",
          data: [
            {
              x: "Soğuk",
              y: 0,
            },
            {
              x: "Soğuk",
              y: 0,
            },
            {
              x: "Soğuk",
              y: 70,
              fillColor: "#7accff"
            },
          ],
        },
      ],
      chartOptions: {
        xaxis: {
          type: "category",
          categories: ["Hedef", "Gerçekleşen", "Beklenen"],
        },
        chart: {
          type: "bar",
          height: 350,
          stacked: true,
        },
        plotOptions: {
          bar: {
            horizontal: true,
          },
        },
      },
    };
  },
};
</script>

<template>
  <apexchart
    type="bar"
    height="350"
    :options="chartOptions"
    :series="series"
  ></apexchart>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
