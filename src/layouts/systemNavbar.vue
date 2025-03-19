<template>
  <wd-config-provider :themeVars="themeVars">
    <view
      class="box-border"
      :style="{
        paddingBottom: `calc(${safeAreaInsets?.bottom}px + 128rpx)`,
      }"
    >
      <slot />
      <view
        class="h-[128rpx] fixed bottom-0 left-0 right-0 bg-[skyblue]"
        :style="{
          paddingBottom: `${safeAreaInsets?.bottom}px`,
        }"
      >
        按钮区域
      </view>
    </view>

    <wd-toast />
    <wd-message-box />
  </wd-config-provider>
</template>

<script lang="ts" setup>
import type { ConfigProviderThemeVars } from 'wot-design-uni'

const { safeAreaInsets } = uni.getWindowInfo()
console.log(123456, safeAreaInsets)
const themeVars: ConfigProviderThemeVars = {
  // colorTheme: 'red',
  // buttonPrimaryBgColor: '#07c160',
  // buttonPrimaryColor: '#07c160',
}
</script>
