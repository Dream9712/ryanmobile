<template>
	<view class="page-container">
		<u-swiper
			class="page-banber"
			:list="bannerList"
			height="130"
		></u-swiper>
		<u-button text="月落"></u-button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				bannerList: [
					'https://img1.baidu.com/it/u=25340056,1897490112&fm=253&fmt=auto&app=120&f=JPEG?w=1422&h=800',
				]
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss" scoped>
	.page-banber {
		width: 100%;
	}
</style>
