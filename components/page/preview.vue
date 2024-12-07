<template>
  <div class="relative h-[100vh] overflow-hidden bg-gray-900 py-24 sm:py-32 flex items-center">
    <img
      alt=""
      src=""
      class="absolute inset-0 -z-10 size-full object-cover object-right md:object-center"
    >
    <div class="mx-auto px-6 lg:px-8">
      <div class="mx-auto lg:mx-0">
        <p class="the-title-preview text-center">{{ value.title }}</p>
        <p class="the-text-preview text-center" :class="{'text-end' : isTextRight}">{{ value.description }}</p>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';

defineProps<{
  value: { title: string, description: string };
  isTextRight: boolean;
}>();
</script>

<style scoped></style>