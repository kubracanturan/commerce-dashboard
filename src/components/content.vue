<template>
  <div class="content">
    <div class="top">
      <v-row>
        <v-col cols="12" sm="8">
          <h1>Welcome, <b>Damian</b></h1>
        </v-col>
        <v-col cols="12" sm="4">
          <SearchMenu/>
        </v-col>
      </v-row>
    </div>
    <div class="">
      <v-row>
        <v-col cols="12" sm="8">
          <OrderProfit/>
          <SalesCharts/>

        </v-col>
        <v-col cols="12" sm="4">
          <TopSelling/>
          <VisitorCharts/>
        </v-col>
      </v-row>
    </div>
  </div>
</template>

<script>
  
  import TopSelling from '../components/topselling';
  import SearchMenu from '../components/searchmenu';
  import OrderProfit from '../components/props';
  import SalesCharts from '../components/salescharts';
  import VisitorCharts from '../components/visitorcharts';
  export default {
    name: 'ContentArea',

    components: {
      SearchMenu, 
      TopSelling, 
      OrderProfit, 
      SalesCharts, 
      VisitorCharts, 
    },

  }
</script>
