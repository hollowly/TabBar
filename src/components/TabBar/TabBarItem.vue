<!--  -->
<template>
	<div class="TabBarItem" @click='itemClick'>
		<slot name='item-icon'></slot>
		<slot name='item-text'></slot>
	</div>
</template>

<script>
export default {
	props: {
		path: String,
	},
	methods: {
		itemClick() {
			this.$router.replace(this.path)
		}
	}

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