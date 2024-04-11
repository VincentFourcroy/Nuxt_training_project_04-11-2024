<template>
  <div class="CustomLayout">
    <Header />
    <p>Custom layout</p>
    <slot />
    <Footer />
  </div>
</template>

<style>
.CustomLayout {
  color: greenyellow;
  background-color: #a79277;
}
</style>
