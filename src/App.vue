<template>
  <div id="app">
    <online-players-table v-bind:info="info"></online-players-table>
    <search></search>
  </div>
</template>

<script>
import 'normalize.css/normalize.css';
import 'font-awesome/css/font-awesome.css';
import HelloWorld from './components/HelloWorld.vue'
import Search from './components/Search.vue';
import OnlinePlayersTable from './components/OnlinePlayersTable.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
    Search,
    OnlinePlayersTable
  },
  data () {
    return {
      info: null,
    }
  },
  mounted() {
    fetch('https://api.bf4stats.com/api/onlinePlayers').then(res => res.json().then(res => this.info = res));
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
  color: #fff;
  font-family: 'Montserrat', sans-serif;
  height: 100vh;
}
</style>
