<template>
  <div id="app">
   <report-component :url="url" :username="username" :password="password"/>
  </div>
</template>

<script>
import ReportComponent from "./components/jasperReport/reportComponent.vue"

export default {
  name: 'App',
  components: {
    ReportComponent
  },
  data(){
    return{
      urlPro:"http://localhost:8082/jasperserver-pro/rest_v2/reports/public/Samples/Reports/Cities.html?",
      url:"http://localhost:8081/jasperserver/rest_v2/reports/reports/interactive/CustomersReport.html?",
      username:"jasperadmin",
      password:"jasperadmin"
    }
  }
}
</script>

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
