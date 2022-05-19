<template>
<div class="ini">
  <div id="nav">
    <Nav> </Nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/index">About</router-link>
  </div>
  </div>
  <router-view />
</template>
<script>
import Nav from "@/components/Nav.vue";
export default {
  name: "App",
  components: {
    Nav,
  },
};
</script>

<style>
#app {
  font-family: "Uni-Sans", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  padding: none;
}

@font-face {
  font-family: "Uni-Sans";
  src: local("Uni-Sans"),
    url(./assets/fonts/UniSansSBold.otf) format("truetype");
}
.ini{
  background-color: rgb(88, 101, 242);
  height: 100vh;
}
#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
