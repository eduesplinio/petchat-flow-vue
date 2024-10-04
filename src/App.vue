<template>
  <div id="app">
    <PetshopHome />
  </div>
</template>

<script>
import PetshopHome from "./components/PetShopHome.vue";

export default {
  name: "App",
  components: {
    PetshopHome,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
