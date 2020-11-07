<!--  -->
<template>
	<div class="TabBarItem">
		<slot></slot>
	</div>
</template>

<script>
export default {
	data () {
		return {

		}
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