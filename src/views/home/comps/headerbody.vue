<template>
  <div class="body">
    <div class="logo">
      <a href="javascript:;">
        <img src="@/assets/img/logo-201305.png" />
      </a>
    </div>
    <div class="search">
      <div class="seartop">
        <form>
          <input type="text" class="text" value="闪购特卖" />
          <input type="button" value="搜索" class="sub" />
        </form>
      </div>
      <div class="searbot">
        <a href="javascript:;" class="active">相机节</a>
        <a href="javascript:;">京东E卡</a>
        <a href="javascript:;">多肉萌宠</a>
        <a href="javascript:;">耐克5折</a>
        <a href="javascript:;">每150减50</a>
        <a href="javascript:;">儿童电动车</a>
        <a href="javascript:;">开衫女</a>
        <a href="javascript:;">1元专享</a>
      </div>
    </div>

    <div class="buy">
      <a href="javascript:;">我的购物车</a>
      <i class="iconfont icon">&#xe61c;</i>
      <div class="nubmer">
        <div class="box">
          0
        </div>
      </div>
    </div>
    <div class="clear"></div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="stylus" scoped>
@import '~@/assets/mixins.styl';

.body {
  mainwidth();
  position relative
  height 80px
  .logo{
    position absolute
    left 0
    top 20px
    }
  .search{
    position absolute
    width: 538px;
    top 20px
    left 400px
    .seartop{
      .text{
        width:446px;
        height: 32px;
        line-height: 32px;
        border: 2px solid #b61d1d;
        float: left;
        padding: 0 4px; color: #666;
        font-size: 14px;
      }
      .sub{
        border 0
        width: 80px;
        height: 36px;
        background: #b61d1d;
        float: left; 
        color: #fff;
        font-size: 16px;
        cursor: pointer;
      }
    } 
    .searbot{
      font-size 12px
      a{
        display inline-block
        padding  10px
      }
    }
  }
  .buy{
    position absolute
    top 25px
    right 50px
    width 120px
    border 1px solid #ccc
    height 30px
    line-height 30px
    font-size 12px
    text-align center
    .nubmer{
      position absolute
      background-color red
      height 14px
      padding 0 3px
      top -5px
      line-height 14px
      left 80px 
      border-radius 14px 14px 14px 0
      color #ffffff
    }
  }
}
.icon{
  font-size 10px
  }
</style>
