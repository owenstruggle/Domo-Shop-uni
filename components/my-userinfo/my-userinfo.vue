<template>
  <view class="my-userinfo-container">

    <!-- 面板的列表区域 -->
    <view class="panel-list">
      <!-- 第一个面板 -->
      <view class="panel">
        <!-- panel 的主体区域 -->
        <view class="panel-body">
          <!-- panel 的 item 项 -->
          <view class="panel-item">
            <text>8</text>
            <text>收藏的店铺</text>
          </view>
          <view class="panel-item">
            <text>14</text>
            <text>收藏的商品</text>
          </view>
          <view class="panel-item">
            <text>18</text>
            <text>关注的商品</text>
          </view>
          <view class="panel-item">
            <text>84</text>
            <text>足迹</text>
          </view>
        </view>
      </view>

      <!-- 第二个面板 -->

      <!-- 第三个面板 -->
    </view>

  </view>
</template>

<script>
  // 按需导入 mapState 辅助函数
  import {
    mapState
  } from 'vuex'
  export default {
    // name: "my-userinfo",
    computed: {
      // 将 m_user 模块中的 userinfo 映射到当前页面中使用
      ...mapState('m_user', ['userinfo']),
    },
    data() {
      return {

      };
    }
  }
</script>

<style lang="scss">
  .my-userinfo-container {
    height: 100%;
    // 为整个组件的结构添加浅灰色的背景
    background-color: #f4f4f4;

    .top-box {
      height: 400rpx;
      background-color: #c00000;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;

      .avatar {
        display: block;
        width: 90px;
        height: 90px;
        border-radius: 45px;
        border: 2px solid white;
        box-shadow: 0 1px 5px black;
      }

      .nickname {
        color: white;
        font-weight: bold;
        font-size: 16px;
        margin-top: 10px;
      }
    }
  }

  .panel-list {
    padding: 0 10px;
    position: relative;
    top: -10px;

    .panel {
      background-color: white;
      border-radius: 3px;
      margin-bottom: 8px;

      .panel-body {
        display: flex;
        justify-content: space-around;

        .panel-item {
          display: flex;
          flex-direction: column;
          align-items: center;
          justify-content: space-around;
          font-size: 13px;
          padding: 10px 0;
        }
      }
    }
  }
</style>
