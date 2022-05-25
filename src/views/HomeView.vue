<template>
  <div>
    <my-head title="购物车案例" background="#1d7bff"></my-head>
    <my-good></my-good>

    <my-foot></my-foot>
  </div>
</template>

<script>

import MyHead from '@/components/MyHead.vue'
import MyGood from '@/components/MyGood.vue'
import MyCount from '@/components/MyCount.vue'
import MyFoot from '@/components/MyFoot.vue'
  export default {
  components: { MyHead, MyGood, MyCount, MyFoot },
  async created(){
    let{ data:res }= await this.$http.get("/api/cart");
    console.log(res)
  }
    
  }
</script>

<style lang="less" scoped>

</style>