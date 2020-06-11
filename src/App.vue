<template>
  <div id="app">
    <router-view/>
    <main-tab-bar/>
  </div>
</template>

<script>
import MainTabBar from '@/components/MainTabBar/MainTabBar'
export default {
    data() {
      return {
      }
    },
    components: {
      MainTabBar
    }
}
</script>

<style>
  @import url('./assets/css/reset.css');
</style>
