<template>
  <div>
    <div
      class="principal"
      v-for="(personaje, index) in personajes"
      :key="index"
    >
      <div><img class="img" :src="personaje.src" alt="Personajes" /></div>
      <p class="text">{{ personaje.nombre }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Personajes",
  data: () => ({
    personajes: [
      {
        nombre: "Rick Sanchez",
        src: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
      },
      {
        nombre: "Morty Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
      },
      {
        nombre: "Summer Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
      },
      {
        nombre: "Beth Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
      },
      {
        nombre: "Jerry Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
      },
    ],
  }),
};
</script>

<style>
.principal {
  display: flex;
  flex-direction: 50%;
  align-items: center;
}

.img {
  width: 150px;
  border-radius: 50%;
  padding: 2rem;
}

.text {
  color: green;
  font-size: 20px;
}
</style>