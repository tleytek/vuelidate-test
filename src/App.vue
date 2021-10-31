<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Composition />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Composition from './components/Composition.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Composition
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
