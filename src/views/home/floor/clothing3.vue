<template>
  <div class="wrap">

    <div class="title">
       <div class="key"> <span>4F</span> 服装鞋包</div>
       <div class="key_item">
         <ul>
           <li><a href="javascript:;" @mousemove="ative=1"  :class="{ative:ative==1}">大牌</a></li>
           <li><a href="javascript:;" @mousemove="ative=2" :class="{ative:ative==2}">男装</a></li>
           <li><a href="javascript:;" @mousemove="ative=3" :class="{ative:ative==3}">女装</a></li>
           <li><a href="javascript:;" @mousemove="ative=4" :class="{ative:ative==4}">鞋靴</a></li>
           <li><a href="javascript:;" @mousemove="ative=5" :class="{ative:ative==5}">箱包</a></li>
           <li><a href="javascript:;" @mousemove="ative=6" :class="{ative:ative==6}">内衣配饰</a></li>
           <li><a href="javascript:;" @mousemove="ative=7" :class="{ative:ative==7}">珠宝首饰</a></li>
           <li><a href="javascript:;" @mousemove="ative=8" :class="{ative:ative==8}">奢品礼品</a></li>
           <li><a href="javascript:;" @mousemove="ative=9" :class="{ative:ative==9}">奢华腕表</a></li>
         </ul>
       </div>
    </div>
  
    <div class="body">
     
     <div class="bd_l1"> 
       <div class="bd_l1_1">
       <div class="bd_l1_item1">
         <div><i></i><a href="">男装</a></div>
         <div><i></i><a href="">女装</a></div>
         <div><i></i><a href="">鞋靴</a></div>
         <div><i></i><a href="">内衣</a></div>
         <div><i></i><a href="">腕表</a></div>
         <div><i></i><a href="">女装</a></div>
         <div><i></i><a href="">腕表</a></div>
         <div><i></i><a href="">女装</a></div>
       </div>
       </div>

     </div>
     <div class="bd_l2">
       <ul v-if="ative==1">
         <li v-for="(item, index) in 8" :key="index">
           <img src="@/assets/img/580db124N73da3744.jpg" alt="">
           <p>杰克琼斯假两件机车修身牛仔夹克</p>
           <div>￥479.40</div>
          </li>
       </ul>
       <ul v-if="ative==2">
         <li v-for="(item, index) in 8" :key="index">
           <img src="@/assets/img/57eb640dN490fc3d3.jpg" alt="">
           <p>杰克琼斯假两件机车修身牛仔夹克</p>
           <div>￥479.40</div>
          </li>
       </ul>
       <ul v-if="ative==3">
         <li v-for="(item, index) in 8" :key="index">
           <img src="@/assets/img/57c54004N3dadba77.jpg" alt="">
           <p>杰克琼斯假两件机车修身牛仔夹克</p>
           <div>￥479.40</div>
          </li>
       </ul>
       <ul v-if="ative==4">
         <li v-for="(item, index) in 8" :key="index">
           <img src="@/assets/img/56f3b5a2N56355d96.jpg" alt="">
           <p>杰克琼斯假两件机车修身牛仔夹克</p>
           <div>￥479.40</div>
          </li>
       </ul>
       <ul v-if="ative==5">
         <li v-for="(item, index) in 8" :key="index">
           <img src="@/assets/img/5803636dNac2f7d5e.jpg" alt="">
           <p>杰克琼斯假两件机车修身牛仔夹克</p>
           <div>￥479.40</div>
          </li>
       </ul>
        <ul v-if="ative==6">
         <li v-for="(item, index) in 8" :key="index">
           <img src="@/assets/img/580da558N562de953.jpg" alt="">
           <p>杰克琼斯假两件机车修身牛仔夹克</p>
           <div>￥479.40</div>
          </li>
       </ul>

       <ul v-if="ative==7">
         <li v-for="(item, index) in 8" :key="index">
           <img src="@/assets/img/56aeecbeNc573c89f.jpg" alt="">
           <p>杰克琼斯假两件机车修身牛仔夹克</p>
           <div>￥479.40</div>
          </li>
       </ul>
       <ul v-if="ative==8">
         <li v-for="(item, index) in 8" :key="index">
           <img src="@/assets/img/578c63ebNc34e2202.jpg" alt="">
           <p>杰克琼斯假两件机车修身牛仔夹克</p>
           <div>￥479.40</div>
          </li>
       </ul>
        <ul v-if="ative==9">
         <li v-for="(item, index) in 8" :key="index">
           <img src="@/assets/img/57d0d141Nc27cbbdc.jpg" alt="">
           <p>杰克琼斯假两件机车修身牛仔夹克</p>
           <div>￥479.40</div>
          </li>
       </ul>

     </div>

     <div class="footer">
       <div class="footer_fl1">

       </div>
       <div class="footer_fl2">
         <ul>
         <li v-for="(item, index) in 4" :key="index">
           <img src="@/assets/img/57ebdfeaNcbe1bd6b.jpg" alt="">
          </li>
       </ul>
       </div>
     </div>

    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      ative:1
    };
  },
  methods: {}
};
</script>

<style lang="stylus" scoped>
@import '~@/assets/mixins.styl';
@import '~@/assets/varibles.styl';
  .ative{
    color red
  }
.wrap{
  mainwidth();
  height 800px

  .title{
    width 100%
    height 40px
    line-height 40px
    overflow hidden
    border-bottom 2px solid red
    .key{
      float left
      height 40px
      box-sizing border-box
      background url('~@/assets/img/nva_bg.png') 18px 5px
      overflow hidden
      span{
        display inline-block
        padding 0 20px
        color #fff
        font-size 12px
      }
    }
    .key_item ul li a{
      float right 
      padding 5px 10px
    }
  }
  .body{
    .bd_l1{
      float left
      width 330px
      height 474px
      overflow hidden
      display flex
      align-items flex-end
      background url('~@/assets/img/57e7e7b5N337c30af.jpg')
      .bd_l1_1{
        width 100%
        background rgba(255,255,255,.5)
        .bd_l1_item1{
         height 80px
         margin-left 3%
         width 95%
         display flex
         flex-wrap wrap
        
       
         div{
          width  25%
          box-sizing border-box
          line-height 40px
          font-size 12px 
          &:nth-of-type(1) i{
           background url('~@/assets/img/clothesicon.png') no-repeat 0px 3.5px;
          }
          &:nth-of-type(2) i{
           background url('~@/assets/img/clothesicon.png') no-repeat 0px 3.5px;
          }
          &:nth-of-type(3) i{
           background url('~@/assets/img/clothesicon.png') no-repeat 0px 3.5px;
          }
          &:nth-of-type(4) i{
           background url('~@/assets/img/clothesicon.png') no-repeat 0px 3.5px;
          }
          &:nth-of-type(5) i{
           background url('~@/assets/img/clothesicon.png') no-repeat 0px 3.5px;
          }

          &:nth-of-type(6) i{
           background url('~@/assets/img/clothesicon.png') no-repeat 0px 3.5px;
          }
          &:nth-of-type(7) i{
           background url('~@/assets/img/clothesicon.png') no-repeat 0px 3.5px;
          }
          &:nth-of-type(8) i{
           background url('~@/assets/img/clothesicon.png') no-repeat 0px 3.5px;
          }
          i{
            display inline-block
            width 30px
            height 30px
            overflow hidden
            vertical-align middle
          }
         }
        }
        .bd_l1_item2{
          background-color pink
          height 100px
          width 100%
        }
      }
    }
    .bd_l2{
      float left
      width 880px
      height 474px
      overflow hidden
      ul li{
       float left 
       cursor pointer
       width 220px
       height 237px
       padding 10px
       box-sizing border-box
       border-right 0.1px solid #f2f2f2
       border-bottom  0.1px solid #f2f2f2
       img{
         display inline-block
         margin-left 30px
       }
       p{
         font-size 12px
         color #666666
       }
       div{
         color red
       }
      }  
    }
    .footer_fl1{
      float left
      cursor pointer
      width 330px
      height 157px
      overflow hidden
      background url('~@/assets/img/57e7e7eaN99f474af.jpg')
    }
    .footer_fl2{
      float left
      width 880px
      height 157px
      overflow hidden
      ul li{
       float left 
       cursor pointer
       box-sizing border-box
       width 220px
       border-bottom  0.1px solid #f2f2f2
       border-right   1px solid #f2f2f2
       img {
         width 100%
       }
      }
    }
  }
}

</style>