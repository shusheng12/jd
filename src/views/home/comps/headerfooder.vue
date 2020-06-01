<template>
  <div class="fooder">
    <div class="bot clearfix">
        <div class="title">全部商品分类</div>
        <ul>
          <li>
            <a href="javascript:;">服装城</a>
          </li>
          <li>
            <a href="javascript:;">美妆馆</a>
          </li>
          <li>
            <a href="javascript:;">京东超市</a>
          </li>
          <li>
            <a href="javascript:;">生鲜</a>
          </li>
          <li>
            <a href="javascript:;">全球购</a>
          </li>
          <li>
            <a href="javascript:;">闪购</a>
          </li>
          <li>
            <a href="javascript:;">团购</a>
          </li>
          <li>
            <a href="javascript:;">拍卖</a>
          </li>
          <li>
            <a href="javascript:;">金融</a>
          </li>
        </ul>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="stylus" scoped>
@import '~@/assets/mixins.styl';

.fooder {
  border-bottom: 3px solid #b1191a;
  margin-top 20px
  .bot {
    mainwidth();
    position relative
    .title{
      width 180px
      background-color #b1191a
      text-align center
      line-height 40px
      color #fff  
    }
    ul {
      position absolute
      top 0
      line-height 40px
      left 200px
      width 600px
      justify-content space-evenly
      display: flex;
    }
  }
}
</style>
