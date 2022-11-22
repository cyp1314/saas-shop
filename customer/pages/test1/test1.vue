<template>
	<view>
		<view style="height: 100px;width: 100vw;background-color: aqua;"></view>
		<view style="height: 100px;width: 100vw;background-color: cadetblue;"></view>
		<view class="header" style="height: 80px;width: 100vw;background-color: indianred;">
			<view style="height: 100%;display: flex;flex-direction: row;align-items: center;justify-content: space-around;">
				<span>体育</span>
				<span>新闻</span>
				<span>娱乐</span>
				<span>游戏</span>
			</view>
		</view>
		<view style="height: 400px;width: 100vw;background-color: aquamarine;display: flex;align-items: center;justify-content: center;font-size: 22px;">
			1
		</view>
		<view style="height: 400px;width: 100vw;background-color: bisque;display: flex;align-items: center;justify-content: center;font-size: 22px;">
			2
		</view>
		<view style="height: 400px;width: 100vw;background-color: cadetblue;display: flex;align-items: center;justify-content: center;font-size: 22px;">
			3
		</view>
		<view style="height: 400px;width: 100vw;background-color: darkcyan;display: flex;align-items: center;justify-content: center;font-size: 22px;">
			4
		</view>
		<view style="margin-bottom: 40px;height: 10px;"></view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="scss">
.header{
	position: sticky;
	top: 0px;
}
</style>
