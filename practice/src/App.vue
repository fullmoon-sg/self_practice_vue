<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <div><basic/><Alert message = "Danger danger Will Robinson" bgcolor="azure"/> 
    <Alert message = "Mary has a little lamb" bgcolor="green"/></div>
    <SayGreetings/>
    <Counter />
    <Alert />
   
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import basic from './components/basic'
import SayGreetings from './components/SayGreetings'
import Counter from './components/Counter'
import Alert from './components/Alert'


export default {
  name: 'App',
  components: {
    HelloWorld, basic, SayGreetings,Counter,Alert
  }
}
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
