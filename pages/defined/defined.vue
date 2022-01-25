<template>
	<view>
		<view>
			组件条件编译：
			<!--  #ifdef  APP-PLUS -->
			APP
			<!--  #endif -->
			<!--  #ifdef  MP-WEIXIN -->
			微信小程序
			<!--  #endif -->
			<!--  #ifdef  H5 -->
			H5
			<!--  #endif -->
		</view>
		<view>
			api条件编译：{{val1}}
		</view>
		<view>
			样式编译：<text class="platform">平台</text>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				val1: ''
			}
		},
		created() {
			this.setVal()
		},
		methods: {
			setVal() {
				// #ifdef  APP-PLUS
				this.val1 = 'APP'
				// #endif
				// #ifdef  MP-WEIXIN
				this.val1 = '微信小程序'
				// #endif
				// #ifdef  H5
				this.val1 = 'H5'
				// #endif
			}
		}
	}
</script>

<style>
	/*  #ifdef  APP-PLUS  */
	.platform {
		color: #007AFF;
	}

	/*  #endif  */
	/*  #ifdef  MP-WEIXIN  */
	.platform {
		color: #4CD964;
	}

	/*  #endif  */
	/*  #ifdef  H5  */
	.platform {
		color: #DD524D;
	}

	/*  #endif  */
</style>
