<script setup lang="ts"></script>

<template>
  <div class="section">
    <span class="chinese-name">鍾佳峻</span>
    <span class="english-name mt-1">James Jhong</span>
    <span class="text-base mt-2">Senior Frontend Engineer</span>
    <div class="contact-box mt-4">
      <div class="flex items-center mt-6">
        <SvgIcon name="icon_email" class="w-4 h-4" />
        <span class="text-sm ml-2">james.jhong.coder@gmail.com</span>
      </div>
      <div class="flex items-center mt-4">
        <SvgIcon name="icon_email" class="w-4 h-4 flex-shrink-0" />
        <span class="ml-2">https://github.com/James-Jhong-Coder</span>
      </div>
    </div>
    <span class="mt-4 leading-tight text-sm"
      >專注於 Vue 生態，擅長大型系統前端架構與使用者體驗設計</span
    >
  </div>
</template>

<style scoped>
  @reference "@/assets/styles/tailwind.css";
  .section {
    @apply flex flex-col;
    @apply leading-none;
  }
  .chinese-name {
    @apply text-2xl text-gray-500;
  }
  .english-name {
    @apply text-base text-gray-300;
  }
  .contact-box {
    @apply flex flex-col;
    @apply text-sm;
  }
</style>
