<template>
  <div id="app">
    <!-- roter-view是单页应用,路由切换时填充内容的容器,换句话说,就是没点击一个路由跳转,我们只是把router-view中的内容替换掉而已 -->
    <router-view></router-view>
    <div class="tabbar">
      <router-link to="/home">首页</router-link>
      <router-link to="/market">闪送超市</router-link>
      <router-link to="/cart">购物车</router-link>
      <router-link to="/mine">我的</router-link>
    </div>
    
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
  #app .tabbar{
    position: fixed;
    left: 0;
    right: 0;
    bottom: 0;
    height: 45px;
    background-color: wheat;
    display: flex;
    align-items: center;
    justify-content: space-around;
  }

</style>
