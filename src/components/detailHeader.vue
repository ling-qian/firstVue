<!-- DetailHeader.vue -->
<template>
  <header class="header">
    <div class="header-inner flexwrap">
        <div id="header-btn-nav" class="header-btn header-btn-back" v-on:click="goBack">
          返回
        </div>
        <div class="header-cont flex">详情</div>
        <div class="header-btn header-btn-cart"></div>
    </div>
  </header>
</template>
<style>
  .flexwrap{display:-webkit-flex;display:flex;}
  .flex{flex:1;}
  .header{height:0.88rem;}
  .header-inner{position:fixed;top:0;left:0;z-index:99;box-sizing:border-box;margin:0 auto;padding:0 0.24rem;border-bottom:0.02rem solid #80ccd6;background-color:#fff;}
  .header-btn-back{line-height:0.86rem;}
  .header-cont{text-align:center;padding:0 0.4rem;line-height:0.86rem;font-size:15px;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;}
  .header-btn:active{opacity:0.7;}
</style>
<script>
  export default {
      methods: {
          goBack() {
              window.history.back();
          }
      }
  }
</script>

