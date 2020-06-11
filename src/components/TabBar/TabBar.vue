<template>
  <div id="tabber">
      <slot></slot>
  </div>
</template>

<script>
export default {
    name: 'TabBar'
}
</script>

<style scoped>
    #tabber {
        width: 100%;
        height: 49px;
        background-color: #f6f6f6;

        position: absolute;
        left: 0;
        right: 0;
        bottom: 0;

        display: flex;
    }
</style>