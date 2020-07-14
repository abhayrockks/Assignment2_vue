<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <mainpage />
  </div>
</template>

<script>
import mainpage from "./components/Mainpage.vue";

export default {
  name: "App",
  components: {
    mainpage
  }
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
