<script setup></script>

<template>
  <header>
    <router-link :to="{ name: 'main'}">main</router-link>
    <router-link :to="{ name: 'fantasy'}">fantasy</router-link>
    <router-link :to="{ name: 'royale'}">royale</router-link>
    <router-link :to="{ name: 'rpg'}">rpg</router-link>
    <router-link :to="{ name: 'shooter'}">shooter</router-link>
    <router-link :to="{ name: 'strategy'}">strategy</router-link>
  </header>
</template>

<style scoped>
header {
  background-color: #ef3e4a;
  color: #15A29C;
  font-size: 20px;
  display: flex;
  justify-content: space-around;
  padding: 20px 0;
  
}
a{
  background:#C02A1B;
  padding: 10px;
  border-radius: 30px;
}
.router-link-active{
   color: #b0d8dc;
}
</style>
