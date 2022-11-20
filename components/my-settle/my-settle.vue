<template>
  <!-- 最外层的容器 -->
  <view class="my-settle-container">
    结算组件
  </view>
</template>

<script>
export default {
  data() {
    return {}
  },
}
</script>

<style lang="scss">
.my-settle-container {
  /* 底部固定定位 */
  position: fixed;
  bottom: 0;
  left: 0;
  /* 设置宽高和背景色 */
  width: 100%;
  height: 50px;
  background-color: cyan;
}
</style>
</style>