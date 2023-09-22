<script lang="ts" setup>
import todos from "../../data/todos.json";
import TodoCard from "../cards/TodoCard.vue";
</script>

<template>
  <section>
    <h1 class="uppercase text-slate-200 font-bold border-s-4 border-s-slate-200 ps-2 mb-2">todos</h1>
    <div class="border border-slate-200">
      <template v-for="todo in todos" :key="todo.id">
        <TodoCard :data="todo" />
      </template>
    </div>
  </section>
</template>

<style scoped>

</style>