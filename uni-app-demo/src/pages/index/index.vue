<template>
  <view class="demo">
    <cl-message ref="message"></cl-message>
    <cl-button @tap="onTap">提示</cl-button>
    <cl-button>默认按钮</cl-button>
    <cl-button type="primary">主要</cl-button>
    <cl-button type="success">成功</cl-button>
    <cl-button type="error">错误</cl-button>
    <cl-button type="warning">警告</cl-button>
    <cl-button type="info">信息</cl-button>
    <cl-button type="text">文本</cl-button>
    <cl-rate :value="2" :color="['#F56C6C', '#E6A23C', '#67C23A']"></cl-rate>
  </view>
</template>

<script>
export default {
  methods: {
    onTap() {
      this.$refs["message"].open({
        message: "hello",
      });
    },
  },
};
</script>