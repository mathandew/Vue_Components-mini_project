<template>
  <div class="app">
    <h1>Components</h1>
    <Counter />
    <ListManager />
  </div>
</template>

<script setup>
import Counter from './components/Counter.vue'
import ListManager from './components/ListManager.vue'
</script>

<style>
.app {
  padding: 2rem;
  font-family: sans-serif;
}
</style>
