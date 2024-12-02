<template>
  <div class="py-4 px-2">
    <div class="the-title-main text-center py-2">Навыки</div>
    <div class="mx-auto grid gap-2 sm:grid-flow-col sm:gap-4 px-4 sm:px-10 lg:px-14">
      <div
        v-for="(item, index) in items"
        :key="index"
        >
        <div class="the-title-secondary text-center py-2">{{ item.title }}</div>
        <div class="the-text-main grid gap-2">
          <p
            v-for="(info, ind) in item.text"
            :key="ind"
          >
            {{ ind+1 }}. {{ info }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps(['title', 'items']);
</script>

<style scoped></style>