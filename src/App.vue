<script setup>
import Header from "./components/Header.vue";
import {RouterView} from "vue-router";
</script>

<template>

  <div class="app">
    <Header />
    <RouterView />
  </div>
</template>

<style>
.app{
  background-color: #C02A1B;
  min-height: 100vh;
}
</style>
