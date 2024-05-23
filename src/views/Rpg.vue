<script setup>
import Card from "../components/Card.vue";
import { GamesCategory } from "../api";
import { onBeforeMount, ref } from "vue";
let games = ref();
onBeforeMount(async () => {
  games.value = await GamesCategory("action-rpg");
  console.log(games);
});
</script>

<template>
  <section>
    <Card v-for="i in games" :key="i.id" :game='i'/>
  </section>
</template>

<style scoped>
section {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 10px;
  padding: 10px;
}
</style>
