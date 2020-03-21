<template>
  <div id="app">
    <div id="topNav">
      <navi></navi>
    </div>
    <div id="centerWrap">
      <div id="st_editor">
        <TextEditor id="myeditor"/>
      </div>
      <div id="st_sidebar"></div>
  </div>
  </div>
</template>

<script>
import TextEditor from './components/TextEditor.vue';
import navi from './components/navi.vue';

export default {
  name: 'App',
  components: {
    TextEditor,
    navi,
  },
};
</script>

<style>
body {
  background-color: #1f2933;
  font-size:16px;
}
.fix{
  clear:both;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0 auto;
  max-width: 1200px;
}
#myeditor {
  background-color: white;
}
</style>
