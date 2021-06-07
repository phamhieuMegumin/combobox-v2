<template>
  <div class="container">
    <Combobox />
  </div>
</template>

<script>
import Combobox from "./components/Combobox.vue";
export default {
  name: "App",
  components: {
    Combobox,
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
  margin-top: 60px;
}
</style>
