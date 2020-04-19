<template>
  <view class="message_block flex_aic">
    <view class="message_icon"><image src="/static/img/avatar0.jpg" mode="aspectFill"></image></view>
    <view class="flex_aic_jcsb message_content">
      <view class="message_info">
        <view>丁酉</view>
        <view>菜鸟果果： 【反倒是佛教圣地佛反对舒服撒到佛山的杰佛森多久教四大覅哦】</view>
      </view>
      <view class="message_time">
        <text v-if="notToday">9月20日</text>
        <text v-else>20:30</text>
      </view>
    </view>
  </view>
</template>

<script>
export default {
  data() {
    return {};
  },

  computed: {
    notToday() {
      return true;
    }
  }
};
</script>

<style lang="scss">
$messageSize: 110upx;
  
.message_block {
  margin: 10upx 20upx;
  margin-right: 0;
  
  .message_icon {
    height: $messageSize - 20;
    width: $messageSize - 20;
    flex-shrink: 0;
    border-radius: 50%;
    overflow: hidden;
    background-color: $uni-color-primary;

    image {
      width: 100%;
      height: 100%;
    }
  }
  
  .message_content {
    flex: 1;
    margin-left: 20upx;
    padding-right: 15upx;
    height: $messageSize;
    border-bottom: 1px solid $uni-text-color-disable;
  }

  .message_info {
    view {
      white-space: nowrap; /*强制内容在一行显示*/
      overflow: hidden; /*超出部分溢出*/
      text-overflow: ellipsis; /*溢出的部分使用省略号*/
      max-width: 450upx;
    }

    view:first-of-type {
      color: $uni-text-color;
      font-size: 30upx;
    }

    view:last-of-type {
      color: $uni-text-color-grey;
    }
  }

  .message_time {
    text-align: center;
    color: $uni-text-color-grey;
  }
}
</style>
