<script setup lang="ts"></script>

<template>
  <div class="page">
    <div class="resume">
      <div class="resume-left">
        <Profile />
        <Divider class="my-4" />
        <Education />
      </div>
      <div class="resume-right">
        <WorkExperience />
        <!-- <span>工作經歷</span>
        <div class="flex flex-col">
          <div class="flex items-center">
            <span>艾克森科技有限公司(在職中)</span>
            <span>Frontend Engineer</span>
          </div>
          <span>2022/06 ~ 現在</span>
          <div>貢獻</div>
          <div class="flex items-center">
            <span>特雷維科技有限公司</span>
            <span>Frontend Engineer</span>
          </div>
          <span>2019/09 – 2022/06</span>
          <div>貢獻</div>
        </div> -->
      </div>
    </div>
  </div>
</template>

<style scoped>
  @reference "@/assets/styles/tailwind.css";
  .page {
    @apply flex flex-col;
    @apply leading-none;
    padding: 10mm 0;
  }
  .resume {
    width: 210mm; /* A4 寬 */
    height: 297mm; /* A4 高 */
    margin: 0 auto;
    @apply bg-white;
    box-shadow: 0 0 6px rgba(0, 0, 0, 0.2);
    @apply flex;
  }
  .resume-left {
    @apply bg-gray-100;
    @apply flex flex-col;
    flex-basis: 35%;
    padding: 8mm;
  }
  .resume-right {
    @apply flex flex-col;
    padding: 8mm;
  }

  .name {
    @apply text-xl;
  }
</style>
