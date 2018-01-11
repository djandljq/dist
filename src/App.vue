<template>
  <div id="app">
  	<div class="search">
  		<span class="iconfont"></span>
  	</div>
   <swiper :list="list" auto style="width:100%;margin:0 auto;" height="200px" :loop="true"></swiper>
  </div>
</template>

<script>
	import { Swiper } from 'vux'
export default {
  name: 'app',
  components:{
  	Swiper
  },
  data(){
  	return {
  		list:[{
			  img: '../static/img/lunbo.jpg',
			}, {
			  img: '../static/img/lunbo1.jpg',
			}, {
			  fallbackImg: '../static/img/lunbo02.jpg'
			}]
  	}
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
html,body{
	width: 100%;
	height: 100%;
	margin: 0;
}
</style>
