<template>
   <div class="shop-cart">
      <div class="header-wrap">
        <div class="header">
          <span class="cart">购物车</span>
          <span class="getCoupon">领券</span>
        </div>
      </div>
      <div class="nav-wrap">
       <ul class="nav">
         <li class="item">
           <i class="iconfont"></i>
           <span class="text">30天无忧退货</span>
         </li>
         <li class="item">
           <i class="iconfont"></i>
           <span class="text">48小时快速退款</span>
         </li>
         <li class="item">
           <i class="iconfont"></i>
           <span class="text">满88元免邮费</span>
         </li>
       </ul>
      </div>
      <div class="cart-content">
          <div class="img-wrap">
            <div class="img"></div>
          </div>
          <div class="login-wrap">
            <div class="add">去添加点什么吧</div>
            <div class="login">登录</div>
          </div>
      </div>
   </div>
</template>
<script>
    export default {
        name: "shop-cart"
    }
</script>

<style scoped lang="stylus">
  .shop-cart
    .header-wrap
      width 100%
      height .88rem
      .header
        height 0.87
        padding 0 .3rem
        line-height 0.87rem
        text-align center
        background-color #fff
        position relative
        .cart
          font-size .36rem
          display inline-block
        .getCoupon
          position absolute
          top 0
          right .6rem
          font-size .3rem
          color #B4282D
    .nav-wrap
      width 100%
      position relative
      z-index 1
      .nav
        height 0.69rem
        padding 0 0.3rem
        display flex
        align-items center
        justify-content space-between
        .item
          font-size 0.12rem
          .iconfont
            display inline-block
            width .09rem
            height .09rem
            background url(//yanxuan-static.nosdn.127.net/hxm/yanxuan-wap/p/20161201/style/img/icon-normal/servicePolicy-1d7541974f.png)
            background-size 100% 100%
    .cart-content
      position fixed
      top .88rem
      left 0
      bottom 0
      z-index 0
      width 100%
      background-color #f4f4f4
      text-align center
      .img-wrap
        position: absolute;
        top: -0.5rem
        right: 0;
        bottom: 0;
        left: 0;
        height: 3rem
        margin: auto;
        .img
          background url(//yanxuan-static.nosdn.127.net/hxm/yanxuan-wap/p/20161201/style/img/icon-normal/noCart-a8fe3f12e5.png)
          display: inline-block;
          vertical-align: middle;
          width: 2.48rem
          height: 2.48rem
          margin-bottom: .08rem
          background-size: 100% 100%
          background-position: center center;
          background-repeat: no-repeat;
      .login-wrap
          width 100%
          height 1.7rem
          position absolute
          top 2.96rem
          right: 0;
          bottom: 0;
          left: 0
          margin auto
          .add
            margin-bottom 0.5rem
            color rgb(153,153,153)
          .login
            width 4.8rem
            height .9rem
            background-color rgb(180,40,45)
            line-height .9rem
            text-align center
            color white
            margin auto
            font-size .3rem
</style>
