<script setup>
import TodoList from '../components/TodoList.vue'
</script>

<template>
  <main>
    <TodoList />
  </main>
</template>

<style>
main {
  border-left: 1px solid var(--color-border);
  padding: 0 2rem;
}
</style>