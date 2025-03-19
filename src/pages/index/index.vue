<!-- 使用 type="home" 属性设置首页，其他页面不需要设置，默认为page；推荐使用json5，更强大，且允许注释 -->
<route lang="json5" type="home">
{
  style: {
    navigationStyle: 'custom',
    navigationBarTitleText: '首页',
  },
}
</route>
<template>
  <view
    class="bg-white border border-[red] border-solid box-border"
    :style="{
      marginTop: safeAreaInsets?.top + 'px',
    }"
  >
    <view @tap="go">系统Navbar</view>
    <view @tap="go2">自定义Navbar-flex布局</view>
    <view @tap="go3">Navbar-fixed布局</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>33333</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>11</view>
    <view>222222</view>
  </view>
</template>

<script lang="ts" setup>
import { TestEnum } from '@/typings'
import PLATFORM from '@/utils/platform'

defineOptions({
  name: 'Home',
})

// 获取屏幕边界到安全区域距离
const { safeAreaInsets } = uni.getWindowInfo()
const author = ref('菲鸽')

// 测试 uni API 自动引入
onLoad(() => {
  console.log(author)
  console.log(TestEnum.A)
})
onMounted(() => {
  console.log('getSystemInfoSync', uni.getSystemInfoSync())
  console.log('getWindowInfo', uni.getWindowInfo())
})

const go = () => {
  uni.navigateTo({
    url: '/pages/other/index',
  })
}
const go2 = () => {
  uni.navigateTo({
    url: '/pages/custom-navbar/index',
  })
}
const go3 = () => {
  uni.navigateTo({
    url: '/pages/custom-navbar-fixed/index',
  })
}
</script>

<style lang="scss" scoped>
.main-title-color {
  color: #d14328;
}
</style>
