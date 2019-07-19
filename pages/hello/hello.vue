<template>
	<navigator url="../index/index" open-type="navigateBack">
	<view class="green" style="width: 750upx; height: 300px;"></view>
	</navigator>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		},
		onLoad() {
			console.log('页面加载')
		},
		onUnload() {
			console.log('页面关闭')
		},
		onReady() {
			console.log('页面初次')
		},
		onShow() {
			console.log('页面show')
		},
		onHide() {
			console.log('页面hide')
		},
		onShareAppMessage() {
			console.log('分享')
		},
		onPageScroll() {
			console.log('滚动')
		},
		onBackPress() {
			console.log('页面返回')
		}
	}
</script>

<style>

</style>
