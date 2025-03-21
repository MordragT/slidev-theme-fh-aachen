<script setup lang="ts">
defineProps<{image: string}>()
</script>

<template>
<div class="h-full grid grid-cols-3">
    <div class="col-span-2">
        <div class="slidev-layout image-right">
            <div class="my-auto">
            <slot />
            </div>
        </div>
    </div>
    <img :src="image" class="object-cover h-full">
</div>
</template>