<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <ComputedPropDemo />
</template>

<script>
import ComputedPropDemo from './components/ComptedPropDemo.vue';

export default {
  name: 'App',
  components: {
    ComputedPropDemo
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
