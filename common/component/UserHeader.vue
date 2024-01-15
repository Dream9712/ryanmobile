<template>
	<view class="app-header">
		<view class="app-header-image">
			<image class="user-image" src="../../static/logo.png" mode=""></image>
			<view class="header-user">
				<view class="user-accout">
					<view class="user-accout-view price-bg">Test001</view>
					<view class="user-accout-view price-bg">ID: test10001</view>
				</view>
				<image class="user-icon" src="../../static/logo.png"></image>
			</view>
		</view>
		<view class="app-header-primary">
			<view class="primary-view">
				<text class="header-text">账户余额:</text>
				<text class="price-bg">200.6k</text>
			</view>
			<view class="primary-view">
				<text class="header-text">冻结余额:</text>
				<text class="price-bg">200.6k</text>
			</view>
		</view>
	</view>
</template>

<script>
</script>

<style lang="scss" scoped>
	.header-text {
		// color: rgba(42, 130, 228, 1);
		// background: linear-gradient(135deg, rgba(66, 189, 255, 1) 0%, rgba(1, 115, 229, 1) 100%);
	}
	.app-header {
		background: linear-gradient(135deg, rgba(66, 189, 255, 1) 0%, rgba(1, 115, 229, 1) 100%);
		color: #fff;
		display: flex;
		font-size: 12rpx;
		
		align-items: center;
		padding: 12rpx 15rpx;
		&-image {
			display: flex;
			align-items: center;
			justify-content: space-between;
			.user-image {
				width: 44rpx;
				height: 44rpx;
				margin: 0 5rpx;
			}
			.user-icon {
				width: 34rpx;
				height: 34rpx;
				margin:0 10rpx 0 20rpx;
			}
		}
		.header-user {
			display: flex;
			align-items: center;
			justify-content: space-between;
			margin:0 10rpx;
			.price-bg {
				padding: 3rpx 11rpx;
			}
			.user-accout-view {
				margin-bottom: 12rpx;
				text-align: center;
			}
		}
		&-primary {
			flex: 1;
			margin-left: 40rpx;
			font-size: 14rpx;
			.header-text {
				margin-right: 5rpx;
			}
			.price-bg {
				padding: 9rpx 20rpx;
			}
			.primary-view {
				margin-bottom: 10rpx;
			}
		}
	}
</style>