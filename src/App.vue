<template>
  <div id="app">
      <router-view></router-view>
      <FoodGuide v-show="$route.meta.isShow"></FoodGuide>
  </div>
</template>

<script>
  import FoodGuide from "./components/FooterGuide/FootGuide"
  export default {
    name: 'App',
    mounted(){
      //this.$store.dispatch("getUser");
    },
    components:{
      FoodGuide
    },
  }
</script>

<style>
</style>
