<template>
  <div class="header-wrap">
    <header class="header">
      <div class="header-content">
        <div class="header-left" @click="$router.replace('/home')">
          <i class="iconfont icon-shouye1"></i>
        </div>
        <slot>
          <div class="header-center">
            <span class="one">发现</span>
            <span>甄选家</span>
          </div>
        </slot>
        <div class="header-right">
          <i class="iconfont icon-sousuo1" @click="$router.replace('/search')"></i>
          <i class="iconfont icon-gouwuche1"></i>
        </div>
      </div>
    </header>
  </div>
</template>

<script>
    export default {
        name: "find-header"
    }
</script>

<style scoped lang="stylus">
  .header-wrap
    height 1rem
    background-color #fafafa
    box-sizing border-box
    border-bottom .01rem solid #d9d9d9
    position fixed !important
    left 0
    top 0
    z-index 99
    width 100%
    .header
      padding 0 .26rem 0 .24rem
    .header-content
      .header-left
        float left
        height 1rem
        line-height 1rem
        i
          font-size 0.5rem
      .header-center
        position: absolute
        width 3.2rem
        height 100%
        line-height 1rem
        text-align center
        left 50%
        top 0
        margin-left -1.6rem
        font-size .28rem
        color #7F7F7F
        z-index 1
        &.img-wrap
          background url("./images/logo.png")
          width 1.6rem
          height 0.48rem
          background-size 100% 100%
          position absolute
          top 0
          right 0
          bottom 0
          left 0
          margin auto
      .one
        display inline-block
        padding 0 0.08rem
        font-size .4rem
        margin-right .2rem
        color: #b4282d;
        font-weight bold
      .two
        display inline-block
        padding 0 0.08rem
      .header-right
        display block
        float right
        height 1rem
        margin-right .02rem
        line-height 1rem
        i
          font-size .5rem
          &:first-child
            margin-right .3rem
          &.last-child
            zoom 1
</style>
