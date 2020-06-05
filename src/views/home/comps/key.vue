<template>
  <div class="key">
    <div class="key1">
      <div v-for="(item, index) in list" :key="index" :class="{item,ative:index===ative}" @click="key(index)">
    <span v-if="index===ative">{{item}}</span><span>{{index+1}}F</span>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    props:{
   ative1:{
     type:Number,
     default:0
   }
  },
    data() {
        return {
            ative:0,
            list:['男装','鞋子','女装','男装']
        }
    },
    methods:{
      key(index){
        this.ative=index
        this.$emit('key',index)
      }
    },
    watch:{
      ative1(){
        this.ative=this.ative1
      }
    }
};
</script>

<style lang="stylus" scoped>

.key
  .key1
    position fixed
    left 50%
    z-index 88888
    margin-left -650px
    top 250px
.item {
  width:35px;
  height: 25px;
  font-size .86rem
  border-bottom  1px  dashed #ccc 
  text-align center
  line-height 25px
  color #666
  cursor pointer
}
.ative{
  background-color red
  color #fff
}
</style>