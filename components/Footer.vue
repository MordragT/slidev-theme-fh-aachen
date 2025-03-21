<script setup lang="ts">
defineProps<{author: string}>()
</script>

<template>
  <div class="bg-dark flex absolute w-full bottom-0 left-0 py-0.5 px-4 text-sm text-white">
    <div class="w-1/3 font-bold">© FH Aachen</div>
    <div class="w-1/3 text-center">{{ author }}</div>
    <div class="w-1/3 text-right">
      <SlideCurrentNo /> / <SlidesTotal />
    </div>
  </div>
</template>