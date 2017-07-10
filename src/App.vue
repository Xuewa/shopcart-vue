<template>
  <div id="app">
    <shopcart :goods="goods"></shopcart>
  </div>
</template>

<script>
import shopcart from './components/shopcart'
const ERR_OK = 0
export default {
  created () {
    console.log(this)
    this.$http.get('/api/goods').then((res) => {
      let response = res.body
      console.log(response)
      if (response.errno === ERR_OK) {
        this.goods = response.data
      }
    })
  },
  data () {
    return {
      goods: []
    }
  },
  components: {
    shopcart: shopcart
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
