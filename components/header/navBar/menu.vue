<template>
  <div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">
    <div class="flex shrink-0 items-center">
      <div>NC</div>
    </div>
    <div class="hidden sm:ml-6 sm:block w-full">
      <div class="flex space-x-8 justify-center">
        <NuxtLink
          v-for="(item, ind) in items"
          :key="ind"
          :class="[item.key === $route.name ? 'nav-link-active' : 'nav-link']"
          :to="item.path"
        >
          {{  item.name }}
        </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';

defineProps<{
  items: { name: string, path: string, key: string }[];
}>();
</script>

<style scoped lang="postcss">
.nav-link-active,
.nav-link {
  @apply relative after:content-[''] after:absolute after:h-[2px] after:right-0 after:bottom-0 after:transition-[width] after:duration-500 py-2 text-sm font-medium;
}

.nav-link-active {
  @apply after:w-full after:bg-red-600 text-white;
}

.nav-link {
  @apply after:w-0 after:bg-red-900 text-gray-300;
}

.nav-link:hover:not(.nav-link-active) {
  @apply hover:after:content-[''] hover:after:absolute hover:after:h-[2px] hover:after:w-full hover:after:left-0 hover:after:bottom-0 hover:after:bg-red-500 hover:after:transition-[width] hover:text-white hover:after:duration-500;
}
</style>