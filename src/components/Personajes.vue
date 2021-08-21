<template>
  <div class="app">
    <div class="principal">
      <img class="img" :src="personajes.src">
      <p class="text">{{ personajes.nombre }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Personajes",
  
  props: { personajes: { type: Object } },

};
</script>

<style>

.principal {
  display: flex;
  flex-direction: 50%;
  align-items: center;
}

.img {
  width: 250px;
  border-radius: 50%;
  padding: 2rem;
}

.text {
  color: green;
  font-size: 20px;
}
</style>