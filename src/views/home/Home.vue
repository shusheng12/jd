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
    <home-key  @key='key' :ative1='ative'/>
    <clothing ref="0"/>
    <clothingo ref="1"  />
    <clothingoo ref="2"  />
    <clothingooo ref="3"  />
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
import Clothing from './floor/clothing'
import Clothingo from './floor/clothing1'
import Clothingoo from './floor/clothing2'
import Clothingooo from './floor/clothing3'
export default {
  components:{
    homeHeaderTop,
    homeHeaderBody,
    homeHeaderFooder,
    homeNavbar,
    homeSwiper,
    homeNews,
    timeLimit,
    homeKey,
    Clothing,
    Clothingo,
    Clothingoo,
    Clothingooo,
  },
  data() {
    return {
      ative:0
    }
  },
  mounted(){
    window.addEventListener('scroll', this.handleScroll)
  },
  methods:{
    key(index){
      this.ani(window,this.$refs[index].$el.offsetTop)
    },
    ani(obj, location, callback) {
			clearInterval(obj.timer)
			obj.timer = setInterval(function () {
        let v = (location - obj.pageYOffset) / 10   
        v = v > 0 ? Math.ceil(v) : Math.floor(v)
				if (v == 1||v==6) {     
					clearInterval(obj.timer)
					if (callback) {
						callback()
					}
				}
        let	y=obj.pageYOffset+v
				window.scrollTo(0,y)
			}, 15)
    },
     handleScroll () {
     var scrollTop = window.pageYOffset || document.documentElement.scrollTop || document.body.scrollTop 
     if(scrollTop<=this.$refs[1].$el.offsetTop)this.ative=0;
     else if(this.$refs[1].$el.offsetTop<scrollTop&&scrollTop<=this.$refs[2].$el.offsetTop) this.ative=1;
     else if(this.$refs[2].$el.offsetTop<scrollTop&&scrollTop<=this.$refs[3].$el.offsetTop) this.ative=2;
     else this.ative=3;
  }
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
