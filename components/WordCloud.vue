<script setup lang="ts">
defineProps<{list: string[]}>()

function randomColor() {
  // see styles/layout.css for the color definitions
  const colors = [
    'var(--slidev-theme-primary)',
    'black',
    'grey',
  ]
  return colors[Math.floor(Math.random() * colors.length)]
}

function randomSize() {
  const min = 2
  const max = 9
  return Math.floor(Math.random() * (max - min + 1) + min)
}
</script>

<template>
  <div>
    <ul aria-label="Word Cloud">
      <li
          v-for="(item, index) in list"
          :style="{
            'font-size': `calc(${randomSize()} * 0.5rem)`,
            color: randomColor(),
          }"
          :key="index">
        {{ item }}
      </li>
    </ul>
  </div>
</template>

<style scoped>
ul {
  @apply list-none px-0 flex flex-wrap items-center justify-center;

  li {
    @apply leading-15 px-2 relative m-0 inline;
  }
}
</style>