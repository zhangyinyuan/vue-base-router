<template>
	<div>
		<textarea id="textarea" class="textarea" v-bind:placeholder="placeholder" v-model="textarea_value"></textarea>
		<br />
		<span style="margin-left: 183px;">您还能输入10个字</span>
		<h1>{{textarea_value}}</h1>
	</div>
</template>

<script>
	console.info("YES");
	export default{
		name:'TestComponent',
		props:{
			placeholder:String
		},
		data(){
			return {
				textarea_value:'',
				title:'请输入文本吧'
			}
		},
		mounted() {},
		methods:{
			selectFunc(value) {
				this.selectValue2 = value
				console.log(this.selectValue)
				console.log(this.selectValue2)
			}
		},
		components:{
			
		}
	}
</script>

<style scoped>
	.textarea{
		width: 300px;
		height: 260px;
	}
</style>