<!-- components/SvgIcon.vue -->
<template>
  <svg aria-hidden="true">
    <use :xlink:href="symbolId" />
  </svg>
</template>

<script setup lang="ts">
  import { computed } from 'vue';

  const props = defineProps<{
    name: string;
  }>();

  const symbolId = computed(() => `#icon-${props.name}`);
</script>
