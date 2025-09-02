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
        <Divider class="my-4" />
        <Skills />
        <Divider class="my-4" />
        <SideProject />
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
    width: 29.7cm;
    height: 21cm;
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
