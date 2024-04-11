<script setup></script>

<template>
  <div class="Header">
    <header>
      <nav>
        <ul>
          <li><NuxtLink to="/" class="link">Home</NuxtLink></li>
          <li><NuxtLink to="/custompage" class="link">Custom</NuxtLink></li>
          <li><NuxtLink to="/state" class="link">State</NuxtLink></li>
          <li>
            <NuxtLink to="/all_properties" class="link">Propriétés</NuxtLink>
          </li>
        </ul>
      </nav>
    </header>
  </div>
</template>

<style lang="scss" scoped>
.Header {
  display: flex;
  background-color: #18122b;
  border-radius: 12px;
}

ul {
  display: flex;
  justify-content: space-around;
  width: 100%;
  list-style: none;
}

.link {
  color: lightgrey;
  display: inline-block;
}
</style>
