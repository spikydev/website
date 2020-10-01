<template>
  <div id="home">
    <div id="mainimage">
      <img
        alt="Vue logo"
        src="../assets/spiky_main_vis_large.png"
        data-aos="zoom-in"
        max-width="850px"
        max-height="479px"
        width="100%"
      />
    </div>
    <HelloWorld
      msg="We develop AI based intelligent solutions for education technologies"
    />
    <h2 id="expTitle">Are you ready to transform education?</h2>
    <h5 id="explanation">
      Most institutions still lack a formal data strategy or practical measures
      in place to advance AI capabilities, which remains a key inhibitor. The
      vast majority of educational leaders understand the need for an AI
      strategy. Our team of AI experts will combine your educational needs and
      produce the right strategy to accelerate your institution into the future
      of education.
    </h5>
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

<style scoped lang="scss">
@import "../assets/colors.scss";

#mainimage {
  display: inline-block;
  vertical-align: top;
  width: 50%;
  padding: 5% 0%;
}
#home {
  width: 100vw;
  height: 100vh;
  padding: 0% 15%;
}

#expTitle {
  color: $expcolor;
}

#explanation {
  color: $expcolor;
  line-height: 2;
  font-weight: 350;
}
</style>
