<template>
  <div id="app">
    <search></search>
  </div>
</template>

<script>
import 'normalize.css/normalize.css';
import 'font-awesome/css/font-awesome.css';
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

#app {
  background: #262626;
  font-family: 'Montserrat', sans-serif;
  height: 100vh;
}
</style>
