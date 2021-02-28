<template>
  <div id="app">
    <Menu />
    <input type="text" v-model="name" />
    <input type="checkbox" v-model="accept" />
    <h1>
      {{ name }}
    </h1>
  </div>
</template>

<script>
import Menu from "./components/Menu.vue";

export default {
  name: "App",
  data() {
    return {
      name: "Mai Khang",
      accept: true,
    };
  },
  components: {
    Menu,
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
