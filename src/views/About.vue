<template>
  <div class="about">
    <h1>This is an about page</h1>
		
		<TestComponent placeholder='请输入内容哦'></TestComponent>
  </div>
</template>

<script>
	import TestComponent from '../components/TestComponent.vue'
	
	export default{
		name:'about',
		components:{
			TestComponent
		}
	}
</script>
