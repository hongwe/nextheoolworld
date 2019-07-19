<template>
	<view>
		
		<view v-for="stuObj in studentArray" :key="stuObj.id">
			
			<checkbox :value="stuObj.name" />{{stuObj.name}}
		</view>
		<button type="primary" @click="addStu()">增加</button>
		
	</view>
</template>

<script>
export default {
	data() {
		return {
			studentArray: [
				{
					id:1,
					name: 'Jack',
					age: 19
				},
				{
					id:2,
					name: 'Steve',
					age: 20
				},
				{
					id:3,
					name: 'Stark',
					age: 18
				}
			]
		};
	},
	methods: {
		addStu(){
			var studentArray = this.studentArray;
			var newId = studentArray.length +1;
			var newStu ={
				id:newId,
				name: '新生'+newId,
				age: 18
			}
			//studentArray.push(newStu);
			studentArray.unshift(newStu);
		}
	}
};
</script>

<style></style>
