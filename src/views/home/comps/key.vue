<template>
  <div class="key">
    <div class="key1">
      <div v-for="(item, index) in 7" :key="index" :class="{item,ative:item===ative}">{{item}}F</div>
    </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            ative:1
        }
    },
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
  height: 35px;
  border-bottom  1px  dashed #ccc 
  text-align center
  line-height 30px
  color #666
  cursor pointer
}
.ative{
  background-color red
  color #fff
}
</style>