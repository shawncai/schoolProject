<template>
	<view class="content">
		<view class="login_title">
			<view class="login_name">登录</view>
			<view class="login_small_name">开启你的校园时光之旅</view>
		</view>
		<view class="login_input">
			<view class="phone_number">
				<view class="left_icon"> 
				<uni-icons type="phone" size="15" color="#000000"  style=" display: flex;align-items: center;justify-content: center;"/>
				</view>
				<view class="right_input">
					<input class="uni-input"  />
				</view>
			</view>
			<view class="phone_number">
				<view class="left_icon">
				<uni-icons type="locked" size="15" color="#000000"  style=" display: flex;align-items: center;justify-content: center;"/>
				</view>
				<view class="right_input">
					<input class="uni-input" password />
				</view>
			</view>
		</view>
		<view class="forget_com">
			<view class="forget_title">忘记密码</view>
			<view class="forget_title">新用户注册</view>
		</view>
		
		<view class="login_button">登录</view>
		
		<view class="tips">手机号快捷登录</view>
		<view class="tips">人脸识别登录</view>
		<view class="third">
			<view class="third_tips">第三方快捷登录</view>
			<view class="other_login">
				<view class="login_item">
					<image src="../../static/qq.png" style="width: 45rpx;height: 45rpx;"></image>
					<view class="item_title">QQ登录</view>
				</view>
				<view class="login_item">
					<image src="../../static/weixin.png" style="width: 45rpx;height: 45rpx;"></image>
					<view class="item_title">微信登录</view>
				</view>
				<view class="login_item">
					<image src="../../static/sinaweibo.png" style="width: 45rpx;height: 45rpx;"></image>
					<view class="item_title">微博登录</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	import uniIcons from '@/components/uni-icons/uni-icons.vue'
	export default {
		comments: {uniIcons},
		data() {
			return {
				
			}
		},
		onLoad() {
			
		},
		methods: {
			
		}
	}
</script>

<style scoped>
	page {
		height: 100vh;
		width: 100%;
	}
	.content {
		width: 100%;
	}
	.login_title {
		height: 25vh;
		display: flex;
		flex-wrap: wrap;
		align-content: center;
		padding-left: 10%;
		color: #333333;
		align-items: center;
	}
	.login_name {
		color: #333333;
		width: 100%;
		font-size: 50rpx;
	}
	.login_small_name {
		width: 100%;
		font-size: 30rpx;
	}
	
	.left_icon {
		width: 30rpx;
		height: 30rpx;
	}
	
	.phone_number {
		padding-left: 10%;
		padding-top: 50rpx;
		display: flex;
		align-items: center;
	}
	
	.login_input {
		width: 100%;
	}
	
	.right_input {
		width: 80%;
		border-bottom: 1px solid #ececec;
	}
	
	.forget_com {
		padding:30rpx 10%;
		padding-right: 15%;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
	
	.forget_title {
		color: #c3c3c3;
		font-size: 25rpx;
	}
	
	.login_button {
		
		width: 80%;
		height: 60rpx;
		margin: 30rpx auto;
		border-radius: 100rpx;
		font-size: 20rpx;
		color: #FFFFFF;
		background-color: #6e29fe;
		display: flex;
		align-items: center;
		justify-content: center;
		
	}
	
	.tips {
		padding-top: 60rpx;
		font-size: 25rpx;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	
	.third {
		padding-top: 10%;
	}
	
	.third_tips {
		width: 100%;
		text-align: center;
		font-size: 20rpx;
	}
	
	.other_login {
		padding-top: 40rpx;
		display: flex;
		align-items: center;
		justify-content: space-around;
	}
	.login_item {
		text-align: center;
	}
</style>