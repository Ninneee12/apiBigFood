<template>
  <HeaderComponent />
  <router-view />
  <FooterComponent />
</template>

<script setup>
import FooterComponent from "@/components/FooterComponent.vue"
import HeaderComponent from "@/components/HeaderComponent.vue"


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
  color: #2c2c2c;
}

nav {
  padding: 30px;
  background-color: rgb(248, 171, 83);
}

nav a {
  font-weight: bold;
  color: #644101;
  text-decoration: none;
}

nav a.router-link-exact-active {
  color: #ffd17c;
}


main {
  margin-top: 0;
  background-color: rgb(255, 255, 255);
  display: flex;
  flex-direction: column;
}

footer {
  display: flex;
  flex-wrap: wrap;
  width: 100%;
  height: 100%;
}

</style>
