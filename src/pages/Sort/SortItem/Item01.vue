<template>
  <div class="sort-right">
    <div class="top-img" :style="{backgroundImage:`url('${categoryList[currentIndex].wapBannerUrl } ')`}">
    </div>
    <div class="sort-list">
      <ul class="list">
        <li class="list-item"
            v-for="subcate in categoryList[currentIndex].subCateList">
          <div class="img-wrap">
            <img :src="subcate.wapBannerUrl">
          </div>
          <div class="name">{{subcate.name}}</div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
    export default {
        name: "item01",
        props:{
          currentIndex:Number,
          categoryList:Array
        }
    }
</script>

<style scoped lang="stylus">
  @import "../../../common/stylus/mixins.styl"
  .sort-right
    width 5.28rem
    margin-left: 1.62rem;
    margin-top 0.88rem
    padding: .3rem .3rem .21rem .3rem
    .top-img
      background url(https://yanxuan.nosdn.127.net/52855d9a0c1f738f26ac125913af0012.jpg?imageView&thumbnail=0x196&quality=75)
      background-size 100% 100%
      width 5.28rem
      height 1.92rem
      margin-bottom 0.32rem
    .sort-list
      .list
        clearFix()
      .list-item
        text-align center
        width 1.44rem
        float left
        margin-right .34rem
        &:nth-child(3n)
          margin-right 0
        .img-wrap
          width 100%
          height 1.44rem
          img
            width 100%
            height 100%
        .name
          width 100%
          height 0.72rem
          font-size 0.24rem
</style>
