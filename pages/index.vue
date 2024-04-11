<script setup lang="ts">
function switchCustomLayout() {
  setPageLayout('custom')
}
definePageMeta({
  layout: 'default',
})

//appel d'un composable
const { sayHello } = useUtils()
sayHello()

//appel d'un plugin
const { $sayHello } = useNuxtApp()
$sayHello('WASSUUUUUUUUUUUUP')

await $fetch('/api/hello')
</script>

<template>
  <div class="Main">
    <h1>Main Page</h1>
    <button @click="switchCustomLayout">Switch layout</button>
    <Alert />
    <ContentDoc />
    <!-- <img src="/image.png" alt="random image" /> -->
    <!-- <img src="/hell.jpg" alt="random image" /> -->
    <!-- <IconsBluetooth /> -->
  </div>
</template>
