<template>
  <div class="top">
    <div class="inner">
      <div class="diqu">送至：北京</div>
      <ul>
        <li>
          <a href="javascript:;">你好，请登录</a>
        </li>
        <li class="zhu">
          <a href="javascript:;">免费注册</a>
        </li>
        <li class="line"></li>
        <li>
          <a href="javascript:;">我的订单</a>
        </li>
        <li class="line"></li>
        <li class="active_bg">
          <a href="javascript:;">
            我的京东
           <i class="iconfont icon">&#xe60c;</i>
          </a>
        </li>
        <li class="line"></li>
        <li>
          <a href="javascript:;">京东会员</a>
        </li>
        <li class="line"></li>
        <li>
          <a href="javascript:;">企业采购</a>
        </li>
        <li class="line"></li>
        <li class="active_bg">
          <a href="javascript:;">
            <span></span>手机京东
            <i class="iconfont icon">&#xe60c;</i>
          </a>
        </li>
        <li class="line"></li>
        <li class="active_bg">
          <a href="javascript:;">
            关注京东
           <i class="iconfont icon">&#xe60c;</i>
          </a>
        </li>
        <li class="line"></li>
        <li class="active_bg">
          <a href="javascript:;">
            客户服务
           <i class="iconfont icon" >&#xe60c;</i>
          </a>
        </li>
        <li class="line"></li>
        <li class="active_bg">
          <a href="javascript:;">
            网站导航
            <i class="iconfont icon">&#xe60c;</i>
          </a>
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

.top {
  background-color: #f1f1f1;
  font-size: 12px;
  height: 30px;
  line-height: 30px;
  color #666

  .inner {
    mainwidth();
    display: flex;
    justify-content: space-between;
    .diqu{
      gestures()
      }
    ul {
      display: flex;
      .line {
        width: 1px;
        height: 10px;
        margin:  10px;
        background-color #ddd
      }
      .zhu{
        margin-left 10px
        a{
          color red
        }
        }
    }
  }
}
.icon{
  font-size 10px
  }
</style>
