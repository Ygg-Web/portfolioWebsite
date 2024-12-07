<template>
  <div class="mx-auto py-4 px-2">
    <div class="the-title-main text-center py-2">{{ title }}</div>
    <div class="the-text-main px-4 sm:px-10 lg:px-14 grid gap-2">
      <p v-for="(item, index) in text" :key="index">
        {{ item }}
      </p>
    </div>
  </div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';

defineProps<{
  title: string;
  text: string[];
}>();
</script>

<style scoped></style>