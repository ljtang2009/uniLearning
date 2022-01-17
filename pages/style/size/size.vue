<template>
	<page-meta root-font-size="32px">
	</page-meta>
	<view class="content">
		<view class="rpx">
			32rpx
		</view>
		<view class="rem">
			1rem
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
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
		padding-top: 20rpx;
	}

	.rpx {
		font-size: 32rpx;
	}

	.rem {
		font-size: 1rem;
	}
</style>
