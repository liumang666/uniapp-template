<route lang="json5" type="page">
{
  layout: 'default',
  style: {
    navigationBarTitleText: '自定义NavBar',
    navigationStyle: 'custom',
  },
}
</route>

<template>
  <view
    class="bg-white overflow-hidden border border-[red] border-solid box-border flex flex-col"
    :style="{
      height: `100vh`,
      paddingBottom: safeAreaInsets?.bottom + 'px',
      paddingTop: safeAreaInsets?.top + 'px',
    }"
  >
    <view class="h-[44px] flex items-center relative">
      <view
        class="absolute top-0 left-0 w-[44px] h-[44px] flex items-center justify-center"
        @tap="back"
      >
        <wd-icon name="thin-arrow-left" size="36rpx"></wd-icon>
      </view>
      <view class="w-[50%] mx-auto h-[44px] leading-[44px] text-center truncate">
        自定义NavBar自定义NavBar自定义NavBar
      </view>
    </view>
    <view class="flex-auto overflow-y-auto border border-[blue] border-solid box-border">
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>1231</view>
      <view>5555555555</view>
    </view>
    <view class="h-[128rpx] shrink-0 bg-[skyblue]">按钮区域</view>
  </view>
</template>

<script lang="ts" setup>
const { safeAreaInsets } = uni.getWindowInfo()
console.log(uni.getWindowInfo())

const back = () => {
  uni.navigateBack()
}
</script>

<style lang="scss" scoped>
//
</style>
