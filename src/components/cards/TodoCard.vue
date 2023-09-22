<script lang="ts" setup>
const props = defineProps({
  data: {
    type: Object,
  }
})
</script>

<template>
  <div class="border-b border-b-slate-600 bg-slate-400 p-4 min-h-[180px]">
    <h2 class="text-2xl font-semibold">{{ data?.task_title }}</h2>
    <!-- <p>{{ data?.task_description }}</p> -->
    <p class="text-sm">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repellendus sint id natus.</p>
  </div>
</template>

<style scoped></style>