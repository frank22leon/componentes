<template>
  <div>
    <Personajes />
  </div>
</template>

<script>
import Personajes from "./components/Personajes.vue";

export default {
  name: "App",
  components: {
    Personajes,
  },
};
</script>

<style>
body {
  background-image: url("https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png");
  background-repeat: no-repeat;
  background-size: cover;
}
</style>