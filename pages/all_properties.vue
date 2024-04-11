<script setup lang="ts">
const runtimeConfig = useRuntimeConfig()
const { data: properties } = await useFetch(
  `${runtimeConfig.public.allproperties}`,
)
</script>

<template>
  <h1>Liste des propriétés</h1>
  <div class="all_cards">
    <div v-for="property in properties" :key="property.id">
      <div class="card">
        <div class="card_content">
          <h3 class="card_title">{{ property.name }}</h3>
          <p class="card_description">
            {{ property.values }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.all_cards {
  display: flex;
  flex-wrap: wrap;
  width: fit-content;
  justify-content: space-around;
  background-color: #18122b;
  border-radius: 25px;
  padding: 0.3rem;
  margin: 1.5rem;

  & .card {
    display: flex;
    justify-content: center;
    width: 200px;
    height: 200px;
    background-color: #393053;
    color: lightgrey;
    border-radius: 25px;
    padding: 2rem;
    margin: 1rem;
  }

  & .card_title {
    text-align: center;
    background-color: #18122b;
    color: lightgrey;
    border-radius: 25px;
    padding: 0.5rem;
  }
}
</style>
