<template>
    <div>
        <div class="header">
            <div class="header-left">
             <span class="iconfont">&#xe624;</span>
             </div>
            <div class="header-input">
            <span class="iconfont">&#xe632;</span>
            输入城市/景点/游玩主题</div>
           <router-link to="/city"> 
            <div class="header-right">{{this.$store.state.city}}
            <span class="iconfont arrow-icon">&#xe64a;</span>
            </div>
            </router-link>
        </div>
    </div>
</template>
<script>
export default {
    name: 'HomeHeader',
    props:{
      swiperList:Array
    }
}

</script>
<style lang="stylus" scoped>
 @import '../assets/variblus.styl'
.header
    display: flex
    line-height: $headerHeight
    background: $bgColor
    color: #fff
    .header-left
      width: .64rem
      float: left
      text-align center
      .back-icon
        text-align: center
        font-size: .4rem
    .header-input
      flex: 1
      height: .64rem
      line-height: .64rem
      margin-top: .12rem
      margin-left: .2rem
      padding-left: .2rem
      background: #fff
      border-radius: .1rem
      color: #ccc
    .header-right
      min-width: 1.04rem
      padding: 0 .1rem
      float: right
      text-align: center
      color: #fff
      .arrow-icon
        margin-left: -.04rem
        font-size: .24rem
</style>