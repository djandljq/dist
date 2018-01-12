<template>
  <div id="app">
  	
  	<!--搜索-->
  	<div class="search">
  		<span class="iconfont"></span>
  		<input type="text" placeholder="搜索保险产品" />
  	</div>
  	
  	<!--轮播图-->
   <swiper :list="list" auto style="width:100%;margin:0 auto;" height="200px" :loop="true"></swiper>
   <!--导航-->
   <div class="navList">
   	<ul>
   		<li>
   			<img src="../static/img/index_nav1.png" />
   			<p>保险分类</p>
   			</li>
   		<li>
   			<img src="../static/img/index_nav2.png" />
   			<p>长期寿险</p>
   			</li>
   		<li>
   			<img src="../static/img/index_nav3.png" />
   			<p>车险</p>
   			</li>
   		</ul>
   		<ul>
   		<li>
   			<img src="../static/img/index_nav4.png" />
   			<p>资讯</p>
   			</li>
   		<li>
   			<img src="../static/img/index_nav5.png" />
   			<p>服务</p>
   			</li>
   		<li>
   		<img src="../static/img/index_nav6.png" />
   			<p>我的中心</p>
   		</li>
   	</ul>
   </div>
   <div class="boxcolor"></div>
   <div class="hangyixian">
   	<p>国民推荐</p>
   	<img src="../static/img/hangyixian.jpg" alt="" />
   </div>
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
}
html,body{
	width: 100%;
	height: 100%;
	margin: 0;
}

p{
	margin: 0;
	padding: 0;
}
ul{
	margin: 0;
	padding: 0;
	list-style: none;
}
/*搜索*/
.search{
	width: 70%;
	height: 2rem;
	line-height: 2rem;
	background:rgba(255,255,252,.5);
	border-radius: 2rem;
	position:fixed;
	top: 0.5rem;
	left: 3.8rem;
	z-index: 20;
	text-align: center;
}
.search input{
	border: none;
	background: none;
	width: 70%;
	height: 60%;
	outline: none;
}

/*导航*/
.navList{
	padding: 0 0.63rem;
	box-sizing: border-box;
}
.navList ul{
	padding-top: 0.8rem;
	display: flex;
}
.navList ul li{
	width: 33.33%;
	flex-wrap: wrap;
	text-align: center;
}
.navList ul li img{
	width: 3rem;
	height: 3rem;
}
.navList ul li p{
		font-size: 0.7rem;
}
.boxcolor{
	width: 100%;
	height: 0.8rem;
	background: #bcbcbc;
}
.hangyixian{
	text-align: center;
	font-size: 0.8rem;
}
.hangyixian p{
	padding: 0.5rem 0;
}
.hangyixian img{
	width: 100%;
	display: block;
}
</style>
