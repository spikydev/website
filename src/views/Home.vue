<template>
  <div class="home">
    <img
      alt="Vue logo"
      src="../assets/spiky_main_vis_large.png"
      data-aos="zoom-in"
    />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld
  }
};
</script>

<style scoped></style>
