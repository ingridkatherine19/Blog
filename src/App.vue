<template>
  <div id="app">
    <TextEditor id="myeditor"/>
  </div>
</template>

<script>
import TextEditor from './components/TextEditor.vue';

export default {
  name: 'App',
  components: {
    TextEditor,
  },
};
</script>

<style>
body {
  background-color: darkcyan;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#myeditor {
  background-color: white;
}
</style>
