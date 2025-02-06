<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count1 = ref(0)
const count2 = ref(0)
const count3 = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  <body>
    <h2>Eggs</h2>
    <button type="button" @click="count1--">-</button>
    <h2>{{ count1 }}</h2>
    <button type="button" @click="count1++">+</button>
    <h2>Milk</h2>
    <button type="button" @click="count2--">-</button>
    <h2>{{ count2 }}</h2>
    <button type="button" @click="count2++">+</button>
    <h2>Lettuce</h2>
    <button type="button" @click="count3--">-</button>
    <h2>{{ count3 }}</h2>
    <button type="button" @click="count3++">+</button>
  </body>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>