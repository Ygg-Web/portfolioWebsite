<template>
  <div class="flex flex-col min-h-[100vh]">
    <HeaderNavBar />
    <main class="flex-initial h-full">
      <slot />
    </main>
    <FooterInfo />
  </div>
</template>

<script setup lang="ts">

</script>

<style scoped></style>
