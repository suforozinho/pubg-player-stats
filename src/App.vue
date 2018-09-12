<template>
  <div id="app">
    <search></search>
  </div>
</template>

<script>
import 'normalize.css/normalize.css';
import HelloWorld from './components/HelloWorld.vue'
import Search from './components/Search.vue';

export default {
  name: 'app',
  components: {
    HelloWorld,
    Search
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Montserrat');

* {
  -webkit-box-sizing: border-box;
     -moz-box-sizing: border-box;
          box-sizing: border-box;
}

body {
  background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('./assets/pubg-background.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  height: 100vh;
}

#app {
  font-family: 'Montserrat', sans-serif;
}
</style>
