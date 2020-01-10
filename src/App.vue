<template>
  <div id="app">
    <router-view></router-view>
    <tab-bar>
      <tab-bar-item path="/home">
        <img slot="item-icon" src="./assets/imgs/tabbar/home.svg" alt="">
        <img slot="item-icon-active" src="./assets/imgs/tabbar/home_active.svg" alt="">
        <div slot="item-text">首页</div>
      </tab-bar-item>
      <tab-bar-item  path="/category">
        <img slot="item-icon" src="./assets/imgs/tabbar/category.svg" alt="">
        <img slot="item-icon-active" src="./assets/imgs/tabbar/category_active.svg" alt="">
        <div slot="item-text">分类</div>
      </tab-bar-item>
      <tab-bar-item path="/shopcart">
        <img slot="item-icon" src="./assets/imgs/tabbar/shopcart.svg" alt="">
        <img slot="item-icon-active" src="./assets/imgs/tabbar/shopcart_active.svg" alt="">
      <div slot="item-text">购物车</div>
      </tab-bar-item>
      <tab-bar-item path="/profile">
        <img slot="item-icon" src="./assets/imgs/tabbar/profile.svg" alt="">
        <img slot="item-icon-active" src="./assets/imgs/tabbar/profile_active.svg" alt="">
      <div slot="item-text">我的</div>
      </tab-bar-item>
    </tab-bar>
  </div>
</template>

<script>
import tabBar from './components/tabbar/tabBar'
import TabBarItem from './components/tabbar/TabBarItem'
export default {
  name: 'App',
  components: {
    tabBar,
    TabBarItem
  }
}
</script>

<style>
@import "./assets/css/base.css"
</style>
