<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld :msg="count"/>
    <button id="btn" @click="incrementCont">{{name}}</button>
    <MyButton :name="name" :contador="count"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import MyButton from './components/MyButton.vue'



export default {
  name: 'App', 
  components: {
    HelloWorld,
    MyButton
},
  data: ()=>({
    count: 0,
    name: 'Aumentar'
  }),
  methods: {
    incrementCont(){
      this.count++
    }
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
