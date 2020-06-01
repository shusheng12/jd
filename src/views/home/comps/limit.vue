<template>
  <div>
    <div class="top"></div>
    <div class="mian">
      <div class="left">
        <h1>京东秒杀</h1>
        <div class="timer">
          <div>{{H}}</div>
          <span>:</span>
          <div>{{M}}</div>
          <span>:</span>
          <div>{{S}}</div>
        </div>
      </div>

      <div class="imglist">
          <img src="@/assets/img/57bd54bfNbc3b4779.jpg" alt="" srcset="">
          <img src="@/assets/img/57bd54bfNbc3b4779.jpg" alt="" srcset="">
          <img src="@/assets/img/57bd54bfNbc3b4779.jpg" alt="" srcset="">
          <img src="@/assets/img/57bd54bfNbc3b4779.jpg" alt="" srcset="">
      </div>
      <div></div>
    </div>
  </div>
</template>

<script>
let th=this;
export default {
  data() {
    return {
      H:0,
      M:0,
      S:0
    };
  },
  mounted() {
   this.timer()
  },
  methods:{
    timer(){
      setInterval(()=>{
      var now = +new Date();
      var set = +new Date("2020-11-1 00:08:00");
      var time = -(now - set) / 1000;
      var h = parseInt((time % (3600 * 24)) / 3600);
      h= h > 9 ? h : "0" + h;
      var m = parseInt((time % 3600) / 60);
      m= m > 9 ? m : "0" + m;
      var s = parseInt(time % 60);
      s = s > 9 ? s : "0" + s;
       this.H = h
       this.M = m
       this.S = s
    }, 1000);
    }
  }
};
</script>

<style lang="stylus" scoped>
@import '~@/assets/mixins.styl';

.top {
  background-color: #f1f1f1;
  font-size: 12px;
  height: 30px;
  line-height: 30px;
  color: #666;
}

.mian {
  mainwidth();
  display flex
  .left {
    box-sizing border-box
    color: #fff;
    height: 180px;
    width: 180px;
    background-color: red;

    h1 {
      margin: 0;
      text-align: center;
      padding-top: 50px;
    }

    .timer {
      display: flex;
      color: #fff;
      margin-top: 30px;
      justify-content: space-evenly;
      text-align: center;
      font-size: 20px;

      div {
        width: 40px;
        height: 40px;
        line-height: 40px;
        background-color: #000;
      }
      span{
        line-height: 40px;
      }
    }
  }
  .imglist{
    flex 1
    display flex
    overflow hidden
    height 195px
    float left 
    img{
      height 100%
    }
  }
}
</style>
