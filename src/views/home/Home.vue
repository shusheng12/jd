<template>
  <div>
    <home-header-top />
    <home-header-body />
    <home-header-fooder />
    <div class="nav">
    <home-navbar />
    <home-swiper />
    <home-news />
    </div>
    <time-limit />
    <home-key />
  </div>
</template>
<script>
import homeHeaderTop from './comps/headertop'
import homeHeaderBody from './comps/headerbody'
import homeHeaderFooder from './comps/headerfooder'
import homeNavbar from './comps/homenavbar'
import homeSwiper from './comps/homeswiper'
import homeNews from './comps/homenews'
import timeLimit from './comps/limit'
import homeKey from './comps/key'
export default {
  components:{
    homeHeaderTop,
    homeHeaderBody,
    homeHeaderFooder,
    homeNavbar,
    homeSwiper,
    homeNews,
    timeLimit,
    homeKey
  }
};
</script>

<style lang="stylus" scoped>
@import '~@/assets/mixins.styl'
  .nav{
    mainwidth()
    display flex
    align-items flex-end 
  }
</style>
