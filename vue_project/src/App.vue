<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h1>{{message}}</h1>
    <firstcomponent></firstcomponent>
    <block></block>
    <router-view/>
  </div>
</template>

<script>
import firstcomponent from './components/firstcomponent.vue'
import block from './components/element.vue'
export default {
  name: 'App',
  data() {
    return {
      message: 'hello,vue!'
    }
  },
  components: { firstcomponent, block }

}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
