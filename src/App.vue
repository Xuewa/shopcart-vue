<template>
  <div id="app">
    <shopcart></shopcart>
  </div>
</template>

<script>
import Shopcart from './components/Shopcart'

export default {
  name: 'app',
  components: {
    shopcart: Shopcart
  }
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
