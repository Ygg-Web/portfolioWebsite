<template>
  <div class="container px-6 py-12 sm:px-12 lg:px-16 mx-auto">
    <div>
      <div class="the-title-main text-center py-2">{{ value.title }}</div>
      <div class="the-text-main">
        <p>
          {{ value.description }}
          <NuxtLink
            to="/projects"
            class="text-[#B8B799]"
          >
            Узнать больше
          </NuxtLink>
        </p>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';

defineProps<{
  value: { title: string, description: string };
}>();
</script>

<style scoped></style>