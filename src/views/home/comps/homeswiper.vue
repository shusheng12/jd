<template>
  <div class="swiper1">
    <swiper
      ref="mySwiper"
      :auto-update="true"
      :auto-destroy="true"
      :delete-instance-on-destroy="true"
      :cleanup-styles-on-destroy="true"
      :options="swiperOptions"
    >
      <swiper-slide>
        <img src="@/assets/img/lunbotu01.jpg" alt />
      </swiper-slide>
      <swiper-slide>
        <img src="@/assets/img/lunbotu02.jpg" alt />
      </swiper-slide>
      <swiper-slide>
        <img src="@/assets/img/lunbotu03.jpg" alt />
      </swiper-slide>
      <swiper-slide>
        <img src="@/assets/img/lunbotu05.jpg" alt />
      </swiper-slide>
      <swiper-slide>
        <img src="@/assets/img/lunbotu06.jpg" alt />
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div> 
       <div class="swiper-button-prev"></div><!--左箭头。如果放置在swiper-container外面，需要自定义样式。-->
    <div class="swiper-button-next"></div><!--右箭头。如果放置在swiper-container外面，需要自定义样式。-->
    </swiper>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import "swiper/css/swiper.css";

export default {
  components: {
    Swiper,
    SwiperSlide
  },
  data() {
    return {
      swiperOptions: {
        pagination: {
          el: ".swiper-pagination"
        },
        autoplay:true,
        loop : true,
        effect : 'cube',
        clickable :true,
        // Some Swiper option/callback...

        
      }
    };
  },
};
</script>

<style lang="stylus" scoped>
@import '~@/assets/mixins.styl';

.swiper1 {
  height: 454px;
  width: 730px;
  overflow hidden
  margin-left 10px
}
.swiper-button-prev{
  position absolute
}
</style>
