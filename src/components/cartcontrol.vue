<template>
  <div class="shopcart">
   <table>
     <thead>
       <tr>
         <th>产品编号</th>
         <th>产品名称</th>
         <th>购买数量</th>
         <th>产品单价</th>
         <th>产品总价</th>
         <th>操作</th>
       </tr>
     </thead>
     <tbody>
       
     </tbody>
   </table>
  </div>
</template>

<script>
export default {
  props (){
    goods: {
      type: Object,
      default: {}
    }
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
