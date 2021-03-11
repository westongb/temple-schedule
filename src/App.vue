<template>
  <div id="app">
    <Header/>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Form/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Header from './components/header.vue'
import Form from './components/form'
export default {
  name: 'App',
  components: {
    HelloWorld,
    Header,
    Form
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
