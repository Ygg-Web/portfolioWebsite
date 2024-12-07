<template>
  <!-- Mobile menu, show/hide based on menu state. -->
  <div class="sm:hidden" id="mobile-menu">
    <div class="space-y-1 px-2 pb-3 pt-2">
      <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
      <NuxtLink to="/" class="block rounded-md bg-gray-900 px-3 py-2 text-base font-medium text-white"
        aria-current="page">Главная</NuxtLink>
      <NuxtLink to="/about"
        class="block rounded-md px-3 py-2 text-base font-medium text-gray-300 hover:bg-gray-700 hover:text-white">
        Резюме</NuxtLink>
      <NuxtLink to="/projects"
        class="block rounded-md px-3 py-2 text-base font-medium text-gray-300 hover:bg-gray-700 hover:text-white">
        Проекты</NuxtLink>
      <NuxtLink to="/contacts"
        class="block rounded-md px-3 py-2 text-base font-medium text-gray-300 hover:bg-gray-700 hover:text-white">
        Контакты</NuxtLink>
    </div>
  </div>
</template>

<script setup lang="ts">

</script>

<style scoped></style>