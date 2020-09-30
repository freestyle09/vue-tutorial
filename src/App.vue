<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Welcome to Your Vue.js App" />
  <Todos v-bind:todos="todos"></Todos>
  <h1>{{ msg }}</h1>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Todos from "./components/Todos.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    Todos
  },
  data() {
    return {
      todos: [
        { id: 1, title: "Todo One", completed: false },
        { id: 2, title: "Todo Two", completed: false },
        { id: 3, title: "Todo Three", completed: false }
      ]
    };
  }
};
</script>

<style>
/* Global styles */
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

body {
}
</style>
