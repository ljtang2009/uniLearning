<template>
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view class="text-area">
			<text class="title">{{title}}</text>
		</view>
		<navigator url="/pages/style/size/size">
			<button type="default">跳转到 尺寸单位</button>
		</navigator>
		<navigator url="/pages/style/backageImage/backageImage">
			<button type="default">跳转到 背景图片</button>
		</navigator>
		<navigator url="/pages/style/icon/icon">
			<button type="default">跳转到 图标字体</button>
		</navigator>
		<navigator url="/pages/defined/defined">
			<button type="default">跳转到 条件编译</button>
		</navigator>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
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
