<template>
  <img alt="Vue logo" src="./assets/vue.svg" />
  <HelloWorld msg="Hello Vue 3 + Vite" />
  <div v-for="item in [1, 2, 3]">
    {{ item }}
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
};
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
