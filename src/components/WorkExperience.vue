<template>
  <div class="section">
    <span class="text-2xl text-gray-400">工作經驗</span>
    <div class="timeline mt-4">
      <div class="timeline-item">第一份工作</div>
      <div class="timeline-item mt-4">第二份工作</div>
      <div class="timeline-item mt-4">第三份工作</div>
    </div>
  </div>
</template>

<style scoped>
  @reference "@/assets/styles/tailwind.css";
  .section {
    @apply flex flex-col;
    @apply leading-none;
  }
  .timeline {
    @apply relative flex flex-col text-sm; /* 預留左邊空間 */
  }
  .timeline::before {
    content: '';
    @apply absolute w-[2px] h-full bg-gray-900;
    top: 7px;
    left: 4px;
    bottom: 7px;
    z-index: 10;
  }

  .timeline-item {
    @apply flex relative pl-4;
  }
  .timeline-item::before {
    content: '';
    @apply absolute w-2 h-2 rounded-full bg-gray-900 border-2 border-white;
    left: 0;
    top: 6px;
  }
</style>
