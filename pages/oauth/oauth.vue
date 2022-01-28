<template>
	<view>
		<view>
			<button type="default" @click="getProvider()">获取第三方服务</button>
			<button @click="wechatLogin()">微信登录</button>
		</view>
		<view>
			<textarea v-model="apiResponse"></textarea>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				apiResponse: ''
			}
		},
		methods: {
			getProvider() {
				uni.getProvider({
					service: 'oauth',
					success: (res) => {
						this.apiResponse = 'success:' + JSON.stringify(res)
					},
					fail: (err) => {
						this.apiResponse = 'fail:' + JSON.stringify(err)
					}
				})
			},
			wechatLogin() {
				uni.login({
					provider: 'weixin',
					// scopes: 'auth_user',
					onlyAuthorize: false,
					success: (loginRes) => {
						this.apiResponse = JSON.stringify(loginRes)
					}
				});
			}
		}
	}
</script>

<style>

</style>
