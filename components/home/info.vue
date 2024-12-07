<template>
  <div class="container mx-auto px-6 py-12 sm:px-12 lg:px-16 h-[100vh] overflow-hidden">
    <div class="grid lg:grid-flow-col gap-10 mx-auto">
      <div class="lg:w-[400px] lg:h-[800px] bg-slate-600" :class="{ 'lg:order-last' : isImgRight }">
        Изображение
      </div>
      <div>
        <div class="the-title-main py-2">
          {{ value.title }}
        </div>
        <div class="tthe-text-main">
          <p>
            {{ value.description }}
            <NuxtLink to="/about" class="text-[#B8B799]">Узнать больше</NuxtLink>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';

defineProps<{
  value: { title: string, description: string };
  isImgRight: boolean;
}>();
</script>

<style scoped></style>