<script setup>
const counter = useCounter()
</script>

<template>
  <div class="state">
    CounterComponent: {{ counter }}
    <button @click="counter++">+</button>
    <button @click="counter--">-</button>
  </div>
</template>
