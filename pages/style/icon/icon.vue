<template>
	<view>
		<view>
			网络图标
			<view>
				<text class="webIcon">&#xe600;</text>
			</view>
		</view>
		<view>
			本地图标（小于40KB）
			<view>
				<text class="localIcon">&#xe600;</text>
			</view>
		</view>
		<view>
			本地字体（大于40KB, 小程序不支持）
			<view>
				<text class="bigFontLocal">测试test123</text>
			</view>
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
	@font-face {
		font-family: 'iconfont';
		/* Project id 2682259 */
		src: url('https://at.alicdn.com/t/font_2682259_vj62yq0jrii.woff2?t=1626579181727') format('woff2'),
			url('https://at.alicdn.com/t/font_2682259_vj62yq0jrii.woff?t=1626579181727') format('woff'),
			url('https://at.alicdn.com/t/font_2682259_vj62yq0jrii.ttf?t=1626579181727') format('truetype');
	}
	
	@font-face {
		font-family: 'iconfontLocal';
		src: url('~@/static/icon/iconfont.ttf');
	}
	
	@font-face {
		font-family: 'bigFontLocal';
		src: url('~@/static/font/FZXingKXJW.TTF');
	}

	.webIcon {
		font-family: iconfont;
	}
	
	.localIcon {
		font-family: iconfontLocal;
	}
	
	.bigFontLocal {
		font-family: bigFontLocal;
	}
</style>
