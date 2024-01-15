<template>
	<view class="page-container">
		<AppHeader />
		<u-swiper
			class="page-banber"
			:list="bannerList"
			height="130"
		></u-swiper>
		<view class="nav-list">
			<view class="nav-list-li" v-for="item in 8" key="item">
				<image class="li-image" src="../../static/logo.png" mode=""></image>
				<text class="li-text">充值</text>
			</view>
		</view>
		<view class="home-pai">
			<view class="pai-title">
				<text>佣金排行榜</text>
			</view>
			<view class="pai-list">
				<view class="pai-user">
					<image class="pai-user-image" src="../../static/logo.png" mode=""></image>
					<view class="pai-user-content">
						<view>855 42****526</view>
						<view>2023-12-17 14:45:32</view>
					</view>
				</view>
				<view class="pai-price">
					+18888 USDT
				</view>
			</view>
			<view class="pai-list">
				<view class="pai-user">
					<image class="pai-user-image" src="../../static/logo.png" mode=""></image>
					<view class="pai-user-content">
						<view>855 42****526</view>
						<view>2023-12-17 14:45:32</view>
					</view>
				</view>
				<view class="pai-price">
					+18888 USDT
				</view>
			</view>
		</view>
		
		<view class="home-pai">
			<view class="pai-title">
				<text>热门咨询</text>
			</view>
			<view class="pai-list">
				<view class="pai-user">
					<view class="pai-user-content zixun-content">
						<view class="zixun-content-title">信用卡逾期后果</view>
						<view>2023-12-17 14:45:32</view>
					</view>
				</view>
				<view class="pai-zixun">
					<text>1221387  阅读量</text>
					<image class="pai-zixun-image" src="../../static/logo.png" mode=""></image>
				</view>
				
			</view>
		</view>
	</view>
</template>

<script>
	import AppHeader from '@/common/component/AppHeader.vue'
	export default {
		components: {
			AppHeader
		},
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
	.border-class {
		background-color: #fff;
		border-radius: 10rpx;
		border: 1rpx solid #defefe;
	}
	
	.nav-list {
		margin-top: 20rpx;
		display: flex;
		flex-wrap: wrap;
		padding: 5rpx 0;
		background: #fff;
		@extend .border-class;
		&-li {
			display: flex;
			flex-direction: column;
			align-items: center;
			justify-content: center;
			width: 25%;
			font-size: 11rpx;
			.li-image {
				width: 35rpx;
				height: 35rpx;
				margin-bottom: 10rpx;
			}
			margin-bottom: 10rpx;
		}
	}
	
	.home-pai {
		margin-top: 15rpx;
		padding: 6rpx 0;
		@extend .border-class;
		.pai-title {
			font-size: 12rpx;
			padding-left: 20rpx;
		}
		.pai-list {
			margin: 10rpx 50rpx;
			padding: 10rpx 0;
			display: flex;
			justify-content: space-between;
			align-items: center;
			border-bottom: 1rpx solid rgba(187, 187, 187, 1);
			.pai-user {
				display: flex;
				justify-content: space-between;
				align-items: center;
				font-size: 12rpx;
				&-image {
					width: 26rpx;
					height: 26rpx;
					margin-right: 20rpx;
				}
			}
			.pai-price {
				
			}
		}
		
		.zixun-content {
			&-title {
				font-size: 24rpx;
				font-weight: 400;
				margin-bottom: 18rpx;
			}
		}
		.pai-zixun {
			display: flex;
			align-items: flex-end;
			font-size: 12rpx;
			&-image {
				width: 122rpx;
				height: 88rpx;
				margin-left: 30rpx;
			}
		}
	}
</style>
