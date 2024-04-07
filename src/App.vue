<template>
  <Suspense> <!--全局异步挂载-->
    <a-config-provider :locale="zhCN">
      <a-app> <!--全局挂载 message-->
        <GlobalView />
      </a-app>
    </a-config-provider>
  </Suspense>
</template>

<script setup lang="ts">
import GlobalView from "./GlobalView.vue"
import zhCN from "ant-design-vue/es/locale/zh_CN"
</script>
