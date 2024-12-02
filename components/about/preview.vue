<template>
  <div class="relative h-[100vh] overflow-hidden bg-gray-900 py-24 sm:py-32 flex items-center">
    <img alt=""
      src="https://images.unsplash.com/photo-1521737604893-d14cc237f11d?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&crop=focalpoint&fp-y=.8&w=2830&h=1500&q=80&blend=111827&sat=-100&exp=15&blend-mode=multiply"
      class="absolute inset-0 -z-10 size-full object-cover object-right md:object-center">
    <div class="mx-auto px-6 lg:px-8">
      <div class="mx-auto lg:mx-0">
        <p class="text-center text-5xl font-semibold text-white sm:text-7xl lg:text-8xl">{{ value.title }}</p>
        <p class="text-center text-2xl sm:text-4xl lg:text-5xl">{{ value.description }}</p>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps(['value']);
</script>

<style scoped></style>