<template>
	<view class="user-container">
		<UserHeader />
		<view class="page-container">
			<u-cell-group style="width: 100%; margin-top: 24rpx;">
				<u-cell title="个人中心" :isLink="true"></u-cell>
				<u-cell title="收付款账号" :isLink="true"></u-cell>
				<u-cell title="团队信息" :isLink="true"></u-cell>
				<u-cell title="邀请码" :isLink="true"></u-cell>
				<u-cell title="账变记录" :isLink="true"></u-cell>
				<u-cell title="选择语言" :isLink="true"></u-cell>
				<u-cell title="VIP晋升规则" :isLink="true"></u-cell>
				<u-cell title="推出登录" :isLink="true"></u-cell>
			</u-cell-group>
		</view>
	</view>
</template>

<script>
	import UserHeader from '@/common/component/UserHeader.vue'
	export default {
		components: {
			UserHeader
		},
		data() {
			return {
				title: '个人中心'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.logo {
		height: 200rpx;
		width: 200rpx;
		margin-top: 200rpx;
		margin-left: auto;
		margin-right: auto;
		margin-bottom: 50rpx;
	}

	.text-area {
		display: flex;
		justify-content: center;
	}

	.title {
		font-size: 36rpx;
		color: #8f8f94;
	}
</style>
