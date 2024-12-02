<template>
  <div class="mx-auto py-4 px-2">
    <div class="text-center py-2 text-xl sm:text-2xl lg:text-3xl">{{ title }}</div>
    <div class="px-4 sm:px-10 lg:px-14 text-base sm:text-lg lg:text-xl grid gap-2">
      <p v-for="(item, index) in text" :key="index">
        {{ item }}
      </p>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps(['title', 'text']);
</script>

<style scoped></style>