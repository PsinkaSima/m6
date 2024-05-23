<script setup>
import { DetailGame } from "../api";
import { onBeforeMount, ref } from "vue";
import { useRoute } from "vue-router";
let info = ref();
let r = useRoute();
onBeforeMount(async () => {
  info.value = await DetailGame(r.params.id);
  console.log(info);
});
</script>
<template>
  <section>
    <nav>
      <img v-for="s in info.screenshots" :src="s.image" :key="s.id" />
    </nav>
    <h1>
      {{ info.title }}
    </h1>
    <p>
      {{ info.description }}
    </p>
  </section>
</template>

<style scoped>
section {
  padding: 20px;
  color: #b0d8dc;
}
nav {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  grid-gap: 30px;
}
img {
  width: 40%;
  aspect-ratio: 16/9;
  border-radius: 20px;
}
h1 {
  font-size: 35px;
  text-align: center;
  padding-top: 17px;
}
p {
  text-align: center;
  padding-top: 17px;
}
</style>
