<template>
  <Header></Header>
  <router-view />
</template>

<script setup>
import Header from "@/views/Header.vue";
</script>
<style>
* {
  margin: 0;
  padding: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
  background-color: rgb(250, 156, 49);
}

nav a {
  font-weight: bold;
  color: #644101;
  text-decoration: none;
}

nav a.router-link-exact-active {
  color: #ffd17c;
}
</style>
