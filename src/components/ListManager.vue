<template>
  <div class="list-manager">
    <h2>Item List</h2>
    <input v-model="newItem" placeholder="Add item" />
    <button @click="addItem">Add</button>
    <ul>
      <li v-for="(item, index) in items" :key="index">{{ item }}</li>
    </ul>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const newItem = ref('')
const items = ref([])

function addItem() {
  if (newItem.value.trim()) {
    items.value.push(newItem.value)
    newItem.value = ''
  }
}
</script>

<style scoped>
input {
  margin-right: 8px;
}
</style>
