<script setup lang="ts">
defineProps<{
  author: string,
  email: string,
  student: number,
}>()
</script>

<template>
  <div class="slidev-layout end">
    <div class="grid grid-rows-2">
      <div>
        <slot />
      </div>

      <div>
        <p>
          <strong>FH Aachen</strong>
          <br>
          <span>Fachbereich Elektrotechnik und Informationstechnik</span>
          <br>
        </p>
        <p>
          <span>{{ author }}</span>
          <br>
          <span>{{ student }}</span>
          <br>
          <span>{{ email }}</span>
          <br>
        </p>
        <p>www.fh-aachen.de</p>
      </div>
    </div>
  </div>
</template>
  


