<template>
  <div class="news">
      <div class="news1">
        <div class="title">
          <h3>京东快报</h3>
          <a href="javascript:;">更多 ></a>
        </div>
        <ul>
          <li>
            <a href="javascript:;">
              <span>[特惠]</span>红米Note3直降100！抽奖赢电视
            </a>
          </li>
          <li>
            <a href="javascript:;">
              <span>[公告]</span>保定市部分城市配送延迟
            </a>
          </li>
          <li>
            <a href="javascript:;">
              <span>[特惠]</span>进口欧德堡低至两件7.5折
            </a>
          </li>
          <li>
            <a href="javascript:;">
              <span>[公告]</span>因广州图书仓搬仓升级配送延迟
            </a>
          </li>
          <li>
            <a href="javascript:;">
              <span>[特惠]</span>9月囤货 运动、美妆3折起
            </a>
          </li>
        </ul>
      </div>
      <div class="icon">
       <ul>
       	    				<li><a href="javascript:;"><i></i><span>话费</span></a></li>
       	    				<li><a href="javascript:;"><i class="ticket"></i><span>机票</span></a></li>
       	    				<li><a href="javascript:;"><i class="cinema"></i><span>电影票</span></a></li>
       	    				<li><a href="javascript:;"><i class="game"></i><span>游戏</span></a></li>
       	    				<li><a href="javascript:;"><i class="lottery"></i><span>彩票</span></a></li>
       	    				<li><a href="javascript:;"><i class="gas"></i><span>加油卡</span></a></li>
       	    				<li><a href="javascript:;"><i class="hotel"></i><span>酒店</span></a></li>
       	    				<li><a href="javascript:;"><i class="train"></i><span>火车票</span></a></li>
       	    				<li><a href="javascript:;"><i class="crowd"></i><span>众筹</span></a></li>
       	    				<li><a href="javascript:;"><i class="money"></i><span>理财</span></a></li>
       	    				<li><a href="javascript:;"><i class="card"></i><span>礼品卡</span></a></li>
       	    				<li><a href="javascript:;"><i class="white"></i><span>白条</span></a></li>  	    				     	    			
        </ul>
      </div>
      <div class="pic">
        <a href="javascript:;">
          <img src="@/assets/img/577cd92fN2de2d25a.jpg" />
        </a>
      </div>
    </div>
</template>

<script>
export default {};
</script>

<style lang="stylus" scoped>
@import '~@/assets/mixins.styl';

.news {
  position relative
  flex: 1
  height 454px
  overflow hidden
  margin 0 10px
  .news1{
    .title{
      display flex
      justify-content space-between
      border 1px solid #ccc
      font-size 14px
      padding 5px
      color #686868
      border-bottom  1px  dashed #ccc
      h3{
        margin 0
        font-weight 200
      }
    }
    ul{
      border 1px solid #ccc
      border-top none
      padding 5px
      font-size 14px
      li{
        margin 5px 0
        span{
          font-weight 900
        }
      }
    }
  } 
  .icon{
    ul{
      display flex
      flex-wrap wrap
      border-left  1px solid #ccc
      li{
        height 70px
        width 25%
        text-align center
        border-right 1px solid #ccc
        border-bottom 1px solid #ccc
        box-sizing border-box
        i{
          width 25px
          height 25px
          margin 0 auto
          margin-top 10px
          display block  
        } 
         &:nth-of-type(1) i {
            background url('~@/assets/img/icon1.png') no-repeat;
         }
         &:nth-of-type(2) i {
            background url('~@/assets/img/icon1.png') no-repeat 0px -26px;
         }
         &:nth-of-type(3) i {
            background url('~@/assets/img/icon1.png') no-repeat 0px -52px;
         }
         &:nth-of-type(4) i {
            background url('~@/assets/img/icon1.png') no-repeat 0px -77px;
         }
         &:nth-of-type(5) i {
            background url('~@/assets/img/icon1.png') no-repeat 0px -100px;
         }
         &:nth-of-type(6) i {
            background url('~@/assets/img/icon1.png') no-repeat 0px -125px;
         }
         &:nth-of-type(7) i {
            background url('~@/assets/img/icon1.png') no-repeat 0px -150px;
         }
         &:nth-of-type(8) i {
            background url('~@/assets/img/icon1.png') no-repeat 0px -175px;
         }
         &:nth-of-type(9) i {
            background url('~@/assets/img/icon1.png') no-repeat 0px -200px;
         }
         &:nth-of-type(10) i {
            background url('~@/assets/img/icon1.png') no-repeat 0px -225px;
         }
          &:nth-of-type(11) i {
            background url('~@/assets/img/icon1.png') no-repeat 0px -250px;
         }
         &:nth-of-type(12) i {
            background url('~@/assets/img/icon1.png') no-repeat 0px -272px;
         }
      }
    }
  } 
  .pic{
    position absolute
    bottom 0
    left 0
    right 0
   img{
     width 100%
   }  
  }  
}
</style>
