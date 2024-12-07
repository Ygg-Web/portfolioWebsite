<template>
  <div
    class="sm:hidden bg-black"
    :class="{'hidden' : !isOpenMenu}"
  >
    <div class="space-y-1 px-2 pb-3 pt-2">
      <NuxtLink
        v-for="(item, ind) in items"
        :key="ind"
        :class="[item.key === $route.name ? 'nav-link-active' : 'nav-link']"
        :to="item.path"
      >
        {{ item.name }}
      </NuxtLink>
    </div>
  </div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';

defineProps<{
  isOpenMenu: boolean;
  items: { name: string, path: string, key: string }[];
}>();
</script>

<style scoped lang="postcss">
.nav-link-active,
.nav-link {
  @apply block rounded-md px-3 py-2 text-base font-medium;
}

.nav-link-active {
  @apply bg-gray-900 text-white;
}

.nav-link {
  @apply text-gray-400;
}

.nav-link:hover:not(.nav-link-active) {
  @apply hover:bg-gray-700 hover:text-white;
}

</style>