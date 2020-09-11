<template>
  <div id="app">
    <HelloWorld msg="notes of jira frontend" />
    <NotesList />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import NotesList from "./components/NotesList.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    NotesList,
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
