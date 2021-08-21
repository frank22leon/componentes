<template>
  <div>
    <Personajes v-for="(personaje, index) in personajes" :key="index" :personaje="personajes">
  </div>
</template>

<script>
import personajes from "./components/Personajes.vue";

export default {
  name: "App",
  components: {
    personajes,
  },
  data: () => ({
    personajes: [
      {
        nombre: "Rick Sanchez",
        src: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
      },
      {
        nombre: "Rick Sanchez",
        src: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
      },
      {
        nombre: "Rick Sanchez",
        src: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
      },
    ],
  }),
};
</script>
<style></style>