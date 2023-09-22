<script lang="ts" setup>
import Todos from "../../components/Tasks/Todos.vue";
import Pendings from "../../components/Tasks/Pendings.vue";
import Completes from "../../components/Tasks/Completes.vue";
</script>

<template>
  <main class="p-6">
    <div class="grid grid-cols-3 gap-6">
      <Todos />
      <Pendings />
      <Completes />
    </div>
  </main>
</template>

<style scoped></style>