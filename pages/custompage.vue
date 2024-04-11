<script setup lang="ts">
function switchCustomLayout() {
  setPageLayout('default')
}
definePageMeta({
  layout: 'custom',
  // middleware: 'auth',
})
</script>

<template>
  <div class="Custom">
    <h1>Custom Page</h1>
    <button @click="switchCustomLayout">Switch layout</button>
    <Alert />
    <img src="/hell.jpg" alt="random image" />
  </div>
</template>
