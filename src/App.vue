<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <NewList msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import NewList from './components/NewList.vue'

export default {
  name: 'App',
  components: {
    NewList
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
