<template>
  <div>
    <nav-bar />
    <router-view />
    <footer-bar />
  </div>
</template>
<script>
import FooterBar from "./components/FooterBar.vue";
import NavBar from "./components/NavBar.vue";
export default {
  components: { NavBar, FooterBar },
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

/* nav {
  padding: 30px;
} */

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #48cae4;
}
</style>
