<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
//import axios from 'axios'
import jsonp from 'jsonp'
export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data () {
    return {
      age:30,
      data:''
    }
  },
  mounted () {

    //axios -- 会发送一个XHR请求
    //let url = "https://mock.presstime.cn/mock/632b13eab98faa00824e4ee9/example/restful/:id/list";
    /* 
    axios.get(url).then(()=>{

    }) 
    */

    //jsonp -- 只是一段js脚本，没有发送请求
    let url = "https://www.imooc.com/activity/servicetime";
    jsonp(url,(err,res)=>{
      let result = res;
      this.data = result;
    })
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
