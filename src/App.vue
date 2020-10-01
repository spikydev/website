<template>
  <div>
    <Navbar />
    <div>
      <router-view />
    </div>
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";

export default {
  name: "HelloWorld",
  components: { Navbar },
};
</script>

<style lang="scss">
@import "./assets/colors.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50; //2c3e50
  margin: 0px 10%;
  border: white;
}

#nav {
  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: $textcolor;
    }
  }
}
</style>
