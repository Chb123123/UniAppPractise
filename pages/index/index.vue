<template>
	<view class="content">
		<text>你好</text>	
		<text selectable="true">我是练习了两年半的实习生蔡徐坤</text>	
		<text>唱跳rop打篮球</text>
		<text>
			好
		</text>
		<view class="box1" hover-class="box1-style" :hover-stay-time="1000">
			<view hover-class="a">
				手指按下
			</view>
		</view>
		<button class="btnStyle">按钮</button>
		<button type="primary" disabled>按钮</button>
		<button type="primary" plain>按钮</button>
		<button type="primary" :loading="state" @click="clickBtn">加载</button>
		<image src="../../static/logo.png" mode="aspectFit"></image>
		<image src="../../static/logo.png" mode="aspectFill"></image>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello',
				state: false
			}
		},
		onShareAppMessage() {
			console.log('点击了分享按钮')
		},
		onPullDownRefresh() {
			console.log('刷新页面')
		},
		onReachBottom() {
			console.log('滚动到底部')
		},
		onLoad() {
			console.log('11')
		},
		onShow() {
			console.log('Hellow')
		},
		methods: {
			clickBtn() {
				this.state = true
			}
		}
	}
</script>

<style>
	.btnStyle{
		height: 30px;
		background-color: #4CD964;
		font-size: 16px;
		line-height: 30px;
	}
	.box1{
		white: 100px;
		height: 100px;
		background-color: blue;
	}
	.box1-style {
		background-color: red;
	}
	.a{
		color:#007AFF;
		background-color:#4CD964;
	}
	.content {
		/* display: flex; */
		/* flex-direction: column; */
		/* align-items: center; */
		/* justify-content: center; */
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
