<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <!-- try type "thisDataPropertyWillNotBeSuggestedByVetur" between the following braces. -->
    <!-- It should suggest "thisDataPropertyWillNotBeSuggestedByVetur" when you type "thisData" but fail-->
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data() {
    return {
      thisDataPropertyWillNotBeSuggestedByVetur: '',
      xxx: ''
    }
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
