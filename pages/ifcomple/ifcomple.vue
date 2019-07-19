<template>
	<view>
		<!-- #ifdef H5 -->
		<view>h5编译</view>
		<!-- #endif -->
		
		<!-- #ifdef APP-PLUS -->
		<view>ios/安卓编译</view>
		<!-- #endif -->
		
		<!-- #ifdef MP -->
		<view>小程序编译</view>
		<!-- #endif -->
		
		<!-- #ifdef MP-WEIXIN -->
		<view>微信小程序编译</view>
		<!-- #endif -->
		
		<!-- #ifndef MP -->
		<view>除去小程序 只在 ios/安卓/h5编译</view>
		<!-- #endif -->
		
		<view class="color"></view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		onLoad(){
			//#ifdef H5
			console.log('h5编译')
			//#endif
			
			
			//#ifdef APP-PLUS
			console.log('ios/安卓编译')
			//#endif
			
			//#ifdef MP
			console.log('小程序编译')
			//#endif
			
			//#ifdef MP-WEIXIN
			console.log('微信小程序编译')
			//#endif
		},
		methods: {
			
		}
	}
</script>

<style>
.color{ 
/*  #ifdef h5 */
background: #080;
/* #endif */

/*  #ifdef APP-PLUS */
background: #020;
/* #endif */

/*  #ifdef MP */
background: #0f0;
/* #endif */

width: 375upx;
height: 375upx;
}
</style>
