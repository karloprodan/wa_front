<template>
  <div id="app">
    <nav-bar :user_status="isLoggedIn" :usr="usr" />
    <search-bar/>
    <router-view :user="usr" :user_status="isLoggedIn" />
    <footer-w/>
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue';
import FooterW from './components/FooterW.vue';
import SearchBar from './components/SearchBar.vue';

export default {
  components: {
    NavBar,
    FooterW,
    SearchBar,
  },


  methods: {

  },
};
</script>

<style lang="scss">
#app {
  font-family: 'Rubik', 'Roboto Slab', Helvetica, Arial, sans-serif;
  font-weight: 400;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  min-height: 100vh;
  position: relative;
  padding-bottom: 150px; // za footer; uglavnom ide visina footera
}
</style>