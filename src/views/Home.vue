<template>
  <div class="home">
    <b-card>
      <b-media no-body>
        <b-media-aside vertical-align="center">
          <img
            alt="Vue logo"
            src="../assets/spiky_main_vis_large.png"
            data-aos="zoom-in"
          />
        </b-media-aside>
        <b-media-body class="ml-3">
          <HelloWorld msg="Welcome to Your Vue.js App" />
        </b-media-body>
      </b-media>
    </b-card>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
  },
};
</script>

<style scoped></style>
