<template>
	<view>
		<input type="text"  style="background: #8f8f8f; height: 100upx;"
		@input="change"
		@focus="focus"
		@blur="blur"
		@confirm="confirm"
		@tap="tap"
		@longpress="longpress"
		@touchstart="touchstart"
		@touchend="touchend"
		@touchmove="touchmove"
		@touchcancel="touchcancel"
		
		>
		<!-- @longtap="longtap" 不推荐 -->
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			// change(e){
			// 	var txtTitle = e.detail.value;
			// 	//debugger;
			// 	this.title= txtTitle;
			// 	
			// 	
			// },
			change(){
				console.log('改变')
			},
			focus(){
				console.log('获得焦点')
			},
			blur(){
				console.log('失去焦点')
			},
			confirm(){
				console.log('回车')
			},
			tap(){
				console.log('触摸离开')
			},
			longpress(){
				console.log('长按')
			},
			//不在推荐使用longtap
			longtap(){
				console.log('长摸')
			},
			
			touchstart(){
				console.log('触摸开始')
			},
			touchend(){
				console.log('触摸结束')
			},
			touchmove(){
				console.log('触摸移动')
			},
			touchcancel(){
				console.log('触摸取消')
			}
			
		}
	}
</script>

<style>

</style>
