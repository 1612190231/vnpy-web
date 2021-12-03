<template>
  <h1 @click="changeMsg">{{msg}}</h1>
  <input type="text" v-model="msg" />
  <div v-bind:id = "id"></div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data(){
	  return{
		  msg:"helloworld",
		  id: "12" 
	  }
  },
  methods:{
	  changeMsg(){
		  this.msg="luck帅呆了！"
		  this.id = "d2"
	  }
  }
}
</script>

<style>
	#d1{
		width:100px;
		
	},
	#d2{
		width: 50px;
	}
</style>