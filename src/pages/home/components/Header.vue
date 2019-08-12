<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe624;</div>
    </div>
    <div class="header-title">
      <span class="iconfont">&#xe632;</span>
      输入城市/景点/游玩主题
    </div>
    <router-link to='/city'>
      <div class="header-right">
        {{this.city}}
        <span class="iconfont arrow-icon">&#xe64a;</span>
    </div>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  props: {
    city: String
  },
  data () {
    return {}
  }
}
</script>

<style lang="stylus" scoped>
  .header
    display flex
    line-height: .88rem
    background: #00bcd4
    color: #fff
    .header-left
      width: .66rem
      text-align: center
      float: left
      .back-icon
        font-size: .34rem
    .header-title
      flex: 1
      height: .66rem
      line-height: .66rem
      margin-top: .12rem
      margin-left: .2rem
      padding-left: .2rem
      background: #fff
      border-radius: .1rem
      color: #ccc
    .header-right
      width: 1.24rem
      float: right
      text-align: center
      color: #fff
      .arrow-icon
        font-size: .15rem
        margin-left: -.03rem

</style>
