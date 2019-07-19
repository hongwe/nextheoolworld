<template>
	<view>
		<!-- v-if v-show区别  移除 和 display:none -->
		<view v-if="isShow">
			now you see me
		</view>
		<view v-else>
			kanbudao
		</view>
		
		<view v-show="isShow">
			kanbudao222
		</view>
		
		<view v-if="sex1 ==1 ? true:false">
			男
		</view>
		
		<view v-if="sex0 ==0 ? true:false">
			女
		</view>
		
		<view>=======================</view>
		
		
		<view v-if="sex3 == 1">
			男
		</view>
		<view v-else-if = "sex3 ==0">
			女
		</view>
		<view v-else>
			不知
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				isShow:true,
				sex0: 0,
				sex1:1,
				sex3:0
			}
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
