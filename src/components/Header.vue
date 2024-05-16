<script setup></script>

<template>
  <header>
    <router-link to="/">main</router-link>
    <router-link to="fantasy">fantasy</router-link>
    <router-link to="royale">royale</router-link>
    <router-link to="rpg">rpg</router-link>
    <router-link to="shooter">shooter</router-link>
    <router-link to="strategy">strategy</router-link>
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
