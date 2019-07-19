<template>
	<view>
		
		<view v-for="(stuObj,stuIndex) in studentArray" :key="stuIndex">
			<view>姓名:{{ stuObj.name }},年龄:{{ stuObj.age }}</view>
			<view>
				技能:
				<!-- <view v-for="sk in stuObj.skill">
					{{ sk }},
				</view> -->
				<block v-for="(sk,skIndex) in stuObj.skill" :key="skIndex">
					{{ sk }},
				</block>
			</view>
		</view>
		
	</view>
</template>

<script>
export default {
	data() {
		return {
			studentArray: [
				{
					name: 'Jack',
					age: 19,
					skill:["A","B","C"]
				},
				{
					name: 'Steve',
					age: 20,
					skill:["A","B","D"]
				},
				{
					name: 'Stark',
					age: 18,
					skill:["B","C"]
				},
				{
					name: 'Jason',
					age: 21,
					skill:["A","B"]
				},
				{
					name: 'Lucy',
					age: 16,
					skill:["A","C"]
				}
			]
		};
	},
	methods: {}
};
</script>

<style></style>
