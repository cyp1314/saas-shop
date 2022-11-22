<template>
	<view class="page">
		<u-navbar :is-back="false" title="购物车" :background="background" title-color="#fff"></u-navbar>
		<view v-if="!hasGoods" class="bg_no_cart">
			<image src="../../static/img/no-cart.png"></image>
			<u-button :custom-style="customStyle" size="mini">随便逛逛</u-button>
		</view>
		<view v-else style="margin-top: 12px;">
			<view v-for="(i,index) in 5" :key="index" style="background-color: #fff;display: flex;align-items: center;margin: 12px 0px;height: 100px;;">
				<view style="height: 100%;width: 24px;margin-right: 12px;display: flex;align-items: center">
					<u-radio active-color="red"></u-radio>
				</view>
				<image style="width: 80px;height: 80px;" mode="aspectFit" src="../../static/logo.png"></image>
				<view style="flex: 1;margin: 0 8px;height: 100px;display: flex;flex-direction: column;justify-content: space-around;">
					<view style="display: flex;">
						<view class="good_title">
							<text>测试测试测试测试测试测测试测试测试测试测试测试测试测试测试测试测试测试测试测试测试测试测试测试测试测试测试测试测试测试测试测试测试测试试测试测试测试测试测试测试测试测试</text>
						</view>
						<u-icon name="weixin" custom-prefix="custom-icon" size="30" color="green"></u-icon>
					</view>
					<view style="margin-top: 4px;display: flex;align-items: center;justify-content: space-between;">
						<text>99.99</text>
						<u-number-box v-model="value" @change="valChange"></u-number-box>
					</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				hasGoods: true,
				value: 0,
				background: {
					backgroundImage: 'linear-gradient(45deg, rgb(28, 187, 180), rgb(141, 198, 63))'
				},
				customStyle: {
					marginTop: '20px', // 注意驼峰命名，并且值必须用引号包括，因为这是对象
					color: 'red'
				}
			};
		},
		methods: {
			valChange(e) {
				console.log('当前值为: ' + e.value)
			}
		}
	}
</script>

<style lang="scss">
	.bg_no_cart {
		height: calc(100vh - 100px);
		width: 100vw;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.good_title {
		font-size: 13px;
		line-height: 26px;
		overflow: hidden;
		text-overflow: ellipsis;
		white-space: wrap;
		display: -webkit-box;
		/* 将对象作为弹性伸缩盒子模型显示 */
		-webkit-line-clamp: 2;
		/* 控制最多显示几行 */
		-webkit-box-orient: vertical;
		/* 设置或检索伸缩盒对象的子元素的排列方式 */
	}
</style>
