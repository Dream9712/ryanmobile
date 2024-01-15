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
			<text class="header-text">余额</text>
			<text class="price-bg">100,000.00</text>
		</view>
	</view>
</template>

<script>
</script>

<style lang="scss" scoped>
	.price-bg {
		font-size: 12rpx;
		font-weight: 500;
		letter-spacing: 1.31rpx;
		color: rgba(255, 255, 255, 1);
		border-radius: 4rpx;
		background: linear-gradient(135deg, rgba(66, 189, 255, 1) 0%, rgba(1, 115, 229, 1) 100%);
	}
	.header-text {
		color: rgba(42, 130, 228, 1);
	}
	.app-header {
		display: flex;
		align-items: center;
		padding: 7rpx 5rpx;
		// justify-content: space-between;
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
				width: 26rpx;
				height: 28rpx;
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
			}
		}
		&-primary {
			flex: 1;
			display: flex;
			align-items: center;
			margin-left: 15rpx;
			.header-text {
				margin-right: 10rpx;
			}
			.price-bg {
				padding: 9rpx 20rpx;
			}
		}
	}
</style>