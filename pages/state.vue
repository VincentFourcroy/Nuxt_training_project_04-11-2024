<script setup>
const counter = useCounter()
</script>

<template>
  <div class="state">
    CounterInPageScript: {{ counter }}
    <button @click="counter++">+</button>
    <button @click="counter--">-</button>

    <div class="counterComponent">
      <Counter />
    </div>
  </div>
</template>
