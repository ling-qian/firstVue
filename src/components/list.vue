<!-- list.vue -->
<template>
  <li class="sec-li">
    <router-link to="/detail" class="lp-li-a">
        <div class="lp-li-imgwrap">
          <img :src="img" alt=""/>
        </div>
      <p class="lp-li-name">{{ title }}</p>
      <p class="lp-li-price">${{ price }}</p>
    </router-link>
  </li>
</template>
<style scoped>
  .sec-li{float:left;width:50%;margin-bottom:0.1rem;}
  .lp-li-a{display:block;padding:0.3rem 0;margin:0 0.05rem;text-align:center;background:#fff;}
  .lp-li-imgwrap{padding:0.24rem 0;}
  .lp-li-imgwrap > img{width:auto;height:2.3rem;}
  .lp-li-name,.lp-li-price{height:0.5rem;line-height:0.5rem;font-size:16px;color:#333;}
  .lp-li-price{color:#fb3b3b;}
</style>
<script>
  export default {
    props: ['price', 'title', 'img']
  }
</script>
