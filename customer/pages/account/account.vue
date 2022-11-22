<template>
	<view class="page">
		<u-navbar :is-back="false" title="会员中心" :background="background" title-color="#fff"></u-navbar>

		<view style="height: 180px;background-color: beige;"></view>
		<view
			style="height: 120px;background-color: aqua;margin: 0 12px;position: relative;top: -20px;border-radius: 4px;">
		</view>
		<view style="border-radius: 4px;height: 220px;background-color: darkcyan;margin: 0 12px;"></view>
		<view style="border-radius: 4px;height: 160px;background-color: darkcyan;margin: 12px 12px;"></view>

		<view style="border-radius: 4px;height: 80px;background-color: forestgreen;margin: 0 12px 80px 12px">
		</view>
		<view style="height: 1px;width: 100vw;"></view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				background: {
					backgroundImage: 'linear-gradient(45deg, rgb(28, 187, 180), rgb(141, 198, 63))'
				},


			};
		}
	}
</script>

<style lang="scss">

</style>
