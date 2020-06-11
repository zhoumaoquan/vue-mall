<template>
   <tab-bar>
      <tab-bar-item link="/home">
        <img slot="tabbar-icon" src="@/assets/img/TabBar/home.svg" alt="">
        <img slot="tabbar-icon-active" src="@/assets/img/TabBar/home_active.svg" alt="">
        <div slot="tabbar-text">首页</div>
      </tab-bar-item>
      <tab-bar-item link="/category">
        <img slot="tabbar-icon" src="@/assets/img/TabBar/category.svg" alt="">
        <img slot="tabbar-icon-active" src="@/assets/img/TabBar/category_active.svg" alt="">
        <div slot="tabbar-text">分类</div>
      </tab-bar-item>
      <tab-bar-item link="/cart">
        <img slot="tabbar-icon" src="@/assets/img/TabBar/cart.svg" alt="">
        <img slot="tabbar-icon-active" src="@/assets/img/TabBar/cart_active.svg" alt="">
        <div slot="tabbar-text">购物车</div>
      </tab-bar-item>
      <tab-bar-item link="/profile">
        <img slot="tabbar-icon" src="@/assets/img/TabBar/profile.svg" alt="">
        <img slot="tabbar-icon-active" src="@/assets/img/TabBar/profile_active.svg" alt="">
        <div slot="tabbar-text">我的</div>
      </tab-bar-item>
    </tab-bar>
</template>

<script>
import TabBar from '@/components/TabBar/TabBar'
import TabBarItem from '@/components/TabBar/TabBarItem'
export default {
    name: 'MainTabBar',
    components: {
      TabBar,
      TabBarItem
    }
}
</script>

<style>

</style>