<template>
  <div class="header">
    <div class="header-left"><i class="iconfont icon-fanhui"></i></div>
    <div class="header-input iconfont icon-sousuo">输入城市/游玩主题</div>
    <div class="header-right"><i class="iconfont icon-xiajiantou"></i>城市</div>
  </div>
</template>
<script>
export default {
  name: 'HomeHeader'
}
</script>
<style lang="stylus" scoped>
    @import '~styles/varibles.styl'
    .header
      background: $bgColor
      line-height: .86rem
      color:#fff
      display: flex
    .header-left
      float: left
      text-align: center
      width:.64rem
    .header-input
      flex: 1
      background-color: #fff
      border-radius:.1rem
      height:.64rem
      margin-top:.12rem
      color:#ccc
      margin-left: .2rem
      line-height: .64rem
      padding-left: .1rem
    .header-right
      float: right
      text-align :center
      width: 1.24rem
</style>

