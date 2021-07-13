<template>
  <div id="app">
    <div class="round">
      <img alt="Vue logo" src="./assets/logo.png" />
    </div>
    <Max msg="Frontend Vue.js App" />
  </div>
</template>

<script>
import Max from "./components/Max.vue";

export default {
  name: "App",
  components: {
    Max,
  },
};
</script>

<style>
body {
  background-color: #e1f5fe;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.round {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 300px;
  height: 300px;
  border-radius: 50%;
  /* padding: 50px; */
  margin: 0 auto;
}

.round:hover {
  box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14),
    0 3px 1px -2px rgba(0, 0, 0, 0.12), 0 1px 5px 0 rgba(0, 0, 0, 0.2);
  cursor: pointer;
}

img {
  transition: 0.5s linear;
  align-items: center;
  margin: 20px;
}
</style>
