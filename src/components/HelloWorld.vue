<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <body>
      <h2>Eggs</h2>
      <button type="button" @click="count--">-</button>
      <h2>{{ count }}</h2>
      <button type="button" @click="count++">+</button>
      <h2>Milk</h2>
      <button type="button" @click="count--">-</button>
      <h2>{{ count }}</h2>
      <button type="button" @click="count++">+</button>
      <h2>Lettuce</h2>
      <button type="button" @click="count--">-</button>
      <h2>{{ count }}</h2>
      <button type="button" @click="count++">+</button>
    </body>
  </div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>