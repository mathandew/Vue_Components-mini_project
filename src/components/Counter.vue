<template>
  <div class="counter">
    <h2>Counter: {{ count }}</h2>
    <button @click="count++">Increase</button>
    <button @click="count--">Decrease</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<style scoped>
.counter {
  margin-bottom: 2rem;
}
button {
  margin-right: 8px;
}
</style>
