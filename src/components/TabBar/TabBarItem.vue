<!--  -->
<template>
	<div class="TabBarItem" @click='itemClick'>
		<slot name='item-icon' v-if='getIsActive'></slot>
		<slot name='item-icon-active' v-else></slot>
		<div :style="getStyle"><slot name='item-text'></slot></div>
	</div>
</template>

<script>
export default {
	props: {
		path: String,
		getColor: {
			type:String,
			default:'red'
		}
	},
	computed: {
		getIsActive() {
			return this.$route.path.indexOf(this.path);
		},
		getStyle() {
			return this.getIsActive ? {} : {'color':this.getColor}
		}
	},
	methods: {
		itemClick() {
			this.$router.replace(this.path)
		},
	},
	


}

</script>

<style>

	.TabBarItem {
		background: #f2f2f2f2;
		height: 49px;
		flex: 1;
		text-align: center;
		font-size: 14px;
	}

	.TabBarItem img {
		width: 24px;
		height: 24px;
		vertical-align: middle;
		margin-top: 3px;
		margin-bottom: 1px;
	}
</style>