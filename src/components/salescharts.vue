<template>
    <div>
        <h3 class="mt-6">Sales Statistics</h3>
        <div id="chart">
          <apexchart type="area" height="350" :options="{
            chart: {
              height: 350,
              type: 'area',
              toolbar: {
                show: false
              },
            },
            colors: ['#FFE5EE', '#C7F2FF'],
            markers: {
                size: 5,
                colors: '#5840BB',
            },
            dataLabels: {
              enabled: false
            },
            stroke: {
              curve: 'smooth'
            },
            xaxis: {
              type: 'text',
              categories: ['Week 1', 'Week 2', 'Week 3', 'Week 4']
            }
          }" :series="[{
            data: [20, 40, 60, 95]
          }, {
            data: [15, 32, 45, 90]
          }]"></apexchart>
        </div>
    </div>
</template>

<script>
  import VueApexCharts from 'vue-apexcharts'

    export default {
      name: 'SalesCharts',
        components: {
          apexchart: VueApexCharts,
        }
    }
  </script>