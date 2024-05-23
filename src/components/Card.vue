<script setup>
defineProps({
  game: Object,
});
</script>

<template>
  <div>
    <img :src="game.thumbnail" />
    <h1>{{ game.title }}</h1>
    <p>
      {{ game.short_description }}
    </p>
    <nav>
      <i class="fas fa-history"></i>
      <span>{{ game.release_date }}</span>
    </nav>
    <nav>
      <i class="fas fa-tv"></i>
      <span>{{ game.platform }}</span>
    </nav>
    <router-link :to="{ name: 'detail', params: { id: game.id } }"
      >Подробнее</router-link
    >
  </div>
</template>

<style scoped>
div {
  width: 100%;
  background-color: #fedac2;
  padding: 20px;
  border-radius: 40px;
  color: #c02a1b;
  display: flex;
  flex-direction: column;
}
img {
  width: 100%;
  object-fit: cover;
  aspect-ratio: 16/9;
  border-radius: 30px;
}
h1 {
  font-size: 30px;
  margin: 10px 0;
}
p {
  font-size: 15px;
  margin-bottom: 10px;
  display: block;
}
nav {
  display: flex;
  font-size: 17px;
  margin-bottom: 10px;
}
i {
  margin-right: 10px;
}
a {
  background-color: #b0d8dc;
  border-radius: 30px;
  font-size: 20px;
  padding: 10px 10px;
  margin-left: auto;
  transition: all 0.5s;
}
a:hover {
  background-color: aqua;
  transform: scale(1.1);
}
</style>
