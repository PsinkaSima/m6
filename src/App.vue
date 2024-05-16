<script setup>
import Header from "./components/Header.vue";
import {RouterView} from "vue-router";
import Card from './components/Card.vue'
</script>

<template>

  <div class="app">
    <Header />
    <RouterView />
    <Card />
  </div>
</template>

<style>
.app{
  background-color: #C02A1B;
  min-height: 100vh;
}
</style>
