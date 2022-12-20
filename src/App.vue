<template>
  <img alt="Vue logo" src="./assets/tee.jpg">
  <h1>{{ fistname }} &nbsp;{{ lanstname }}</h1>
  <h1>{{ nickname }}</h1>
  <h1>{{ age }}</h1>
  <h1>{{ room }}</h1>
  <h1>{{ major }}</h1>
  <h1>{{ school }}</h1>
  <h2>{{ getfullname() }}</h2>
  <h2>{{ hobby }}</h2>
  <ul>
    <li><h2>{{ hobby[0] }}</h2></li>
    <li><h2>{{ hobby[1] }}</h2></li>
    <li><h2>{{ hobby[2] }}</h2></li>
    <li><h2>{{ hobby[3] }}</h2></li>
  </ul>
  <h2>{{ preofile }}</h2>
  <ul>
    <li><h2>{{ preofile.geead }}</h2></li>
    <li><h2>{{ preofile.wrigth }}</h2></li>
    <li><h2>{{ preofile.hight }}</h2></li>
    <li><h2>{{ preofile.status }}</h2></li>
  </ul>
</template>

<script>

export default {
  name : 'App',
  data(){ //เรียกข้อมูลเฉพาะ
    return{
      fistname : "Napat",
      lanstname : "Surin",
      nickname : "Tee",
      age : "20",
      room : "IT.5102",
      major : "No.23",
      school : "LANNA POLYTECHNIC CHIANGMAI",
      hobby : ["01","02","03","04"],//ข้อมูล Array
      preofile  : {geead : "male" , wrigth : 50,hight : 180,status : false}//ข้อมูลวัตถุ
    }
  },
  methods : { //เรียกข้อมูลแบบ Function
    getfullname(){
      return this.fistname + this.lanstname //เรียกค่าจาก data แล้ว return ออกไปเป็น Function getfullname
    }
  }
}
</script>

<style>
#app {
  font-family : Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing : antialiased;
  -moz-osx-font-smoothing : grayscale;
  text-align : center;
  color : #2c3e50;
  margin-top : 60px;
}
</style>
