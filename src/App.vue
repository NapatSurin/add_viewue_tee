<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <h1>{{ fistname }}</h1>
  <h1>{{ lanstname }}</h1>
  <h1>{{ nickname }}</h1>
  <h1>{{ age }}</h1>
  <h1>{{ room }}</h1>
  <h1>{{ major }}</h1>
  <h1>{{ school }}</h1>
</template>

<script>

export default {
  name: 'App',
  data(){
    return{
      fistname:"Napat",
      lanstname:"Surin",
      nickname:"Tee",
      age:"20",
      room:"IT.5102",
      major:"No.23",
      school:"LANNA POLYTECHNIC CHIANGMAI"
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
