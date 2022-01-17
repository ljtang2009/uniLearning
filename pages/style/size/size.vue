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
		<view class="vhvw">
			width: 50vw;
			height: 30vh;
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
	
	.vhvw {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		width: 50vw;
		height: 30vh;
		background-color: #3F536E;
		color: #FFFFFF;
	}
</style>
