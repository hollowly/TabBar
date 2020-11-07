<!--  -->
<template>
	<div>
	<tab-bar>
		<tab-bar-item path='/home'>
			<img src="../../assets/img/TabBar/home.png" slot='item-icon'>
			<div slot='item-text'>首页</div>
		</tab-bar-item>
		<tab-bar-item path='/categories'>
			<img src="../../assets/img/TabBar/categories.png" slot='item-icon'>
			<div slot='item-text'>更多</div>
			</tab-bar-item>
		<tab-bar-item path='/shopcart'>
			<img src="../../assets/img/TabBar/shopcart.png" slot='item-icon'>
			<div slot='item-text'>购物车</div>
			</tab-bar-item>
		<tab-bar-item path='/profile'>
			<img src="../../assets/img/TabBar/profile.png" slot='item-icon'>
			<div slot='item-text'>我的</div>
			</tab-bar-item>
	</tab-bar>
	<keep-alive>
		<router-view></router-view>
	</keep-alive>
	</div>
</template>

<script>
import TabBar from './TabBar'
import TabBarItem from './TabBarItem'
export default {
	components: {
		TabBar,
		TabBarItem
	}
}

</script>

<style>

</style>