<template>
  <div id="home">
    <div id="mainimage">
      <img
        alt="Vue logo"
        src="../assets/spiky_main_vis_large.png"
        data-aos="fade-right"
        max-width="850px"
        max-height="479px"
        width="100%"
      />
    </div>
    <HelloWorld
      msg="We develop AI based intelligent solutions for education technologies"
    />
    <div data-aos="fade-up">
      <h2 id="expTitle">Are you ready to transform education?</h2>
      <h5 id="explanation">
        Most institutions still lack a formal data strategy or practical
        measures in place to advance AI capabilities, which remains a key
        inhibitor. The vast majority of educational leaders understand the need
        for an AI strategy. Our team of AI experts will combine your educational
        needs and produce the right strategy to accelerate your institution into
        the future of education.
      </h5>
    </div>
    <img
      class="segment"
      src="https://images.squarespace-cdn.com/content/v1/5d44ad660d24df00017284b8/1589740638753-FV0AWFQ3Q2OX86NHCHB3/ke17ZwdGBToddI8pDm48kNgFsonEPp3fPfBQwkX3i3lZw-zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZcY1lis3u7ujHaqKviAjfgBXb2P7ACMlJX44aBDLb--x92WTJLha2eVZactBRQOPSaWMf8oKYo5TjNLnzY893erdFHRhJo0VxFpQhBJHTdAQ/segmentify.png"
      alt="segmentify.png"
    />
    <Brands />
    <img
      class="segment"
      src="https://images.squarespace-cdn.com/content/v1/5d44ad660d24df00017284b8/1589740638753-FV0AWFQ3Q2OX86NHCHB3/ke17ZwdGBToddI8pDm48kNgFsonEPp3fPfBQwkX3i3lZw-zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZcY1lis3u7ujHaqKviAjfgBXb2P7ACMlJX44aBDLb--x92WTJLha2eVZactBRQOPSaWMf8oKYo5TjNLnzY893erdFHRhJo0VxFpQhBJHTdAQ/segmentify.png"
      alt="segmentify.png"
    />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import Brands from "@/components/Brands.vue";

export default {
  name: "Home",
  components: {
    HelloWorld,
    Brands,
  },
};
</script>

<style scoped lang="scss">
@import "../assets/colors.scss";

.segment {
  width: 100%;
  padding-top: 3%;
}

hr {
  position: relative;
  top: 20px;
  border: none;
  height: 3px;
  background: #929292;
  margin-bottom: 3%;
}

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
  font-family: "Brown";
}

#explanation {
  color: $expcolor;
  line-height: 2;
  font-family: "Brown Regular";
}
//32 and 20 at start.
@media only screen and (max-width: 965px) {
  #expTitle {
    font-size: 25px;
  }
  #explanation {
    font-size: 15.625px;
  }
}

@media only screen and (max-width: 860px) {
  #expTitle {
    font-size: 20px;
  }
  #explanation {
    font-size: 12.5px;
  }
}

@media only screen and (max-width: 607px) {
  #expTitle {
    font-size: 20px;
  }
  #explanation {
    font-size: 8px;
  }
}
@media only screen and (max-width: 485px) {
  #expTitle {
    font-size: 15px;
  }
  #explanation {
    font-size: 6px;
  }
}

@media only screen and (max-width: 365px) {
  #expTitle {
    font-size: 10px;
  }
  #explanation {
    font-size: 4px;
  }
}
</style>
