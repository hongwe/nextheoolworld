<template>
	<view class="container">
		<view class="green txt" style="height: 200upx; font-size: 30px;">1</view>
		<view class="green txt2" style="font-size: 10px;">2</view>
		<view class="green txt" style="height: 300upx; font-size: 50px;">3</view>


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
.container{
	display: flex;
	flex-direction: row;
	flex-wrap: nowrap;
	/* justify-content:space-around; */
	/* align-items: baseline; */
	align-items: center;
height: 800upx;
	background: #008800;
	}
.green{ background: #00FF00 ;
 
 }
.txt{ font-size: 20px;width: 100upx;}
.txt2{ font-size: 20px;width: 100upx; align-self: center; }
</style>
