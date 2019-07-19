<template>
	
	<view class="content">
		<image class="logo" src="/static/logo.png"></image>
		<view>
			<text class="title">{{title}}</text>
			<input type="text" :value="title" @input="change"/>
			
		</view>
		<view>
			
			<text class="title">{{name}}</text>
		</view>
		
		<navigator v-bind:url="url">
		<view>
			
			I am {{student.age >= 18 ? '成年' :'未成年'}} years old.</br>
			I have skills such as: {{skill[0]}},{{skill[1]}},{{skill[2]}},{{skill[3]}}
		</view>
		</navigator>
		
		<navigator url="../vif/vif">
		<view>
			
			VIF
		</view>
		</navigator>
		
		<navigator url="../vfor/vfor">
		<view>
			
			Vfor
		</view>
		</navigator>
		<navigator url="../vforkey/vforkey">
		<view>
			
			Vforkey
		</view>
		</navigator>
		</navigator>
		<navigator url="../ifcomple/ifcomple">
		<view>
			
			ifcomple
		</view>
		</navigator>
		
		
		<view class="box">
			<navigator url="../flex/flex-direction/flex-direction">
			<view style="width: 150upx;">
				
				flex-direction
			</view>
			</navigator>
			<navigator url="../flex/flex-wrap/flex-wrap">
			<view style="width: 150upx;">
				
				flex-wrap
			</view>
			</navigator>
			<navigator url="../flex/justify-content/justify-content">
			<view style="width: 150upx;">
				
				justify-content
			</view>
			</navigator>
			<navigator url="../flex/align-items/align-items">
			<view style="width: 150upx;">
				
				align-items
			</view>
			</navigator>
			<navigator url="../flex/align-content/align-content">
			<view style="width: 150upx;">
				
				align-content
			</view>
			</navigator>
			<navigator url="../flex/align-items/align-items">
			<view style="width: 150upx;">
				
				align-items
			</view>
			</navigator>
			<navigator url="../flex/align-self/align-self">
			<view style="width: 150upx;">
				
				align-self
			</view>
			</navigator>
		</view>
		
		
		
	</view>
</template>
<!-- 三个标签　每个只能存在一个 -->


<script>
	// vm:协调者 调度器
	export default {
	//model:所有的数据
		data() {
			return {
				title: 'Hello next学院',
				name:'wanghong',
				student:{
					age:18
				},
				skill:["Java","Html","Css","Scloud","Vue"],
				url: '../hello/hello',
				image:'/static/logo.png'
			}
		},
		onLoad() {

		},
		methods: {
change(e){
	var txtTitle = e.detail.value;
	//debugger;
	this.title= txtTitle;
	
	
}
		}
	}
</script>

<style>
	.content {
		text-align: center;
		height: 400upx;
	}

	.logo {
		height: 200upx;
		width: 200upx;
		margin-top: 100upx;
	}

	.title {
		font-size: 36upx;
		color: #8f8f94;
	}
	.box{
		display: flex;
		justify-content: center;
		flex-wrap: wrap;	
			} 
</style>
