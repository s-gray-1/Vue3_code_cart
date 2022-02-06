<template>
  <div class="hearder-container" :style="{ backgroundColor:bgcolor,color:color,fontSize:fsize+'px'}">{{title}}</div>
</template>

<script>
export default {
  name:'EsHeader',
  props:{
    title:{
      type:String,
      default:'es-header'
    },
    bgcolor:{
      type:String,
      default:'#007BFF'
    },
    color:{
      type:String,
      default:'#fff'
    },
    fsize:{
      type:Number,
      default:12
    }
  }
}
</script>

<style lang='less' scoped>
  .hearder-container {
    position: fixed;
    top:0;
    left: 0;
    width: 100%;
    height: 45px;
    text-align: center;
    line-height: 45px;
    z-index: 999;
  }
</style>