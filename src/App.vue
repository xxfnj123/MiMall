<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
//import axios from 'axios'
//import jsonp from 'jsonp'
export default {
  name: 'App',
  components: {
    
  },
  data () {
    return {

    }
  },
  mounted () {

    //axios -- 会发送一个XHR请求
    /*
    let url = "https://mock.presstime.cn/mock/632b13eab98faa00824e4ee9/example/restful/:id/list";
    axios.get(url).then(()=>{

    }) 
    */

    //jsonp -- 只是一段js脚本，没有发送请求
    /*
    let url = "/api/activity/servicetime";
    jsonp(url,(err,res)=>{
      let result = res;
      this.data = result;
    })
    */
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
