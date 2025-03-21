<script setup lang="ts">
defineProps<{author: string}>()
</script>

<template>
  <div class="slidev-layout quote">
    <div data-quote-container class="text-5xl relative mb-2">
      <slot />
    </div>
    <hr class="w-48 border-t-5 border-[var(--slidev-theme-primary)] mb-2" />
    <p v-if="author" class="italic text-xl font-extralight">{{ author }}</p>
  </div>
</template>

<style scoped>
[data-quote-container]::before {
  content: '\„';
  @apply text-8xl absolute -bottom-6 -left-12;
}
</style>