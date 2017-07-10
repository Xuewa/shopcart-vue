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
       <tr v-for="good in goods">
         <td>{{good.prodNo}}</td>
         <td>{{good.prodName}}</td>
         <td><cartcontrol :prodNo="good.prodNo"></cartcontrol></td>
       </tr>
     </tbody>
   </table>
  </div>
</template>

<script>
export default {
  props: {
    goods: {
      type: Array
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
