<!--  -->
<template>
	<div id='TabBar'>
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
	#TabBar {
		display: flex;
		position: fixed;
		left: 0;
		bottom: 0;
		right: 0;
	}
</style>