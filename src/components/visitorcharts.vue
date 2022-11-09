<template>
    <div>
        <h3>Sales Statistics</h3>
        <div id="chart">
          <apexchart type="area" height="150" :options="{
            chart: {
              height: 150,
              type: 'area',
              toolbar: {
                show: false
              },
            },
            colors: ['#5840BB'],
            markers: {
                size: 5,
            },
            dataLabels: {
              enabled: false
            },
            stroke: {
              curve: 'smooth'
            },
            xaxis: {
              type: 'text',
              categories: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
            }
          }" :series="[{
            data: [20, 40, 20, 50, 20, 40, 20 ]
          }]"></apexchart>
        </div>
    </div>
</template>

<script>
  import VueApexCharts from 'vue-apexcharts'

    export default {
      name: 'VisitorCharts',
        components: {
          apexchart: VueApexCharts,
        }
    }
  </script>