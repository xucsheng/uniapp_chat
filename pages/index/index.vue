<template>
	<view class="content">
		<text>首页</text>
		<view>
			<navigator url="/subpages/chat/chat">前往和知心姐姐聊天</navigator>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: '首页'
			}
		},
		onShow() {
			console.log('index page show');
		},
		onLoad() {
           console.log(getCurrentPages());
		},
		onPullDownRefresh() {
			console.log('页面下拉刷新')
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
