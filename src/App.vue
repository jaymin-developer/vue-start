<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld
      v-for="todoItem in todos"
      v-bind:todo="todoItem"
      v-bind:key="todoItem.id"
    />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
  data() {
    return {
      todos: [
        { id: 0, name: "사과" },
        { id: 1, name: "망고" },
        { id: 2, name: "두리안" },
        { id: 3, name: "블루베리" },
      ],
    };
  },
};
</script>

<style>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>
