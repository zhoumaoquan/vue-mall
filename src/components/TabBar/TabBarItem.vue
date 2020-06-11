<template>
  <div class="tabbar-item" @click="routerChange">
      <div v-if="!isActive"><slot name="tabbar-icon"></slot></div>
      <div v-else><slot name="tabbar-icon-active"></slot></div>
      <div :style="isActiveColor"><slot name="tabbar-text"></slot></div>
      
  </div>
</template>

<script>
export default {
    name: 'TabBarItem',
    props: {
        link: String,
        activeColor: {
            type: String,
            default: '#FF5777'
        }
    },
    data() {
        return { 
        }
    },
    computed: {
        isActive() {
            return this.$route.path  == this.link;
        },
        isActiveColor() {
            return this.isActive ? { color:  this.activeColor} : {}
        }
    },
    methods: {
        routerChange() {
            this.$router.push(this.link);
        }
    }
}
</script>

<style scoped>
    .tabbar-item {
        flex: 1;
        text-align: center;
        margin-top: 3px;
        font-size: 14px;
    }
    .tabbar-item img {
        width: 24px;
        height: 24px;
        vertical-align: bottom;
    }
    .active {
       color: #FF5777;
   }
</style>