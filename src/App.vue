<template>
<div id='#app'>
	<tab-bar>
		<tab-bar-item>
			<img src="./assets/img/TabBar/home.png">
			<div>首页</div>
		</tab-bar-item>
		<tab-bar-item>
			<img src="./assets/img/TabBar/categories.png">
			<div>更多</div>
			</tab-bar-item>
		<tab-bar-item>
			<img src="./assets/img/TabBar/shopcart.png">
			<div>购物车</div>
			</tab-bar-item>
		<tab-bar-item>
			<img src="./assets/img/TabBar/profile.png">
			<div>我的</div>
			</tab-bar-item>
	</tab-bar>
</div>
</template>

<script>
import TabBar from './components/TabBar/TabBar'
import TabBarItem from './components/TabBar/TabBarItem'
export default {
	name: 'App',
	components: {
		TabBar,
		TabBarItem
	}
}
</script>

<style>
@import url('./assets/css/base.css');
</style>
