<template>
  <div data-aos="flip-up">
    <h2>Leading Brands Trust Spiky</h2>
    <div id="brands">
      <img id="image" :src="imageURLs[indexOfImg]" :class="classVar" />
    </div>
  </div>
</template>

<script>
var data = {
  indexOfImg: 0,
  imageURLs: [
    "data:image/jpeg;base64,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",
    "https://www.iasp.ws/media/imagegenerator/0x100/upscale(false)/00274_01_bk-mobil-logo.png",
    "https://imgrosetta.mynet.com.tr/file/2293076/728xauto.jpg",
  ],
  classVar: "",
  counter: 0,
};

export default {
  name: "Brands",
  data: function () {
    return data;
  },
  methods: {
    carousel: function () {},
  },
  created() {
    const self = this;
    setInterval(() => {
      self.counter++;
      if (self.counter === 2) {
        self.classVar = "fadeEffect";
        self.indexOfImg = (self.indexOfImg + 1) % 3;
        self.counter = 0;
      } else self.classVar = "";
    }, 1500);
  },
};
</script>

<style scoped lang="scss">
@import "../assets/colors.scss";

.fadeEffect {
  -webkit-animation: fadein 1s; /* Safari, Chrome and Opera > 12.1 */
  -moz-animation: fadein 1s; /* Firefox < 16 */
  -ms-animation: fadein 1s; /* Internet Explorer */
  -o-animation: fadein 1s; /* Opera < 12.1 */
  animation: fadein 1s;
}

#brands {
  //Our frame
  width: 200px;
  height: 200px;
  //border: 1px solid red;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0 auto;
}

#image {
  //image
  max-width: 200px;
  max-height: 200px;
  //border: 1px solid green;
}

h2 {
  color: $expcolor;
  font-family: "Brown Regular";
  text-align: center;
  font-weight: bold;
  padding-bottom: 2%;
}

b-carousel-slide {
  font-family: "Brown Regular";
}

@keyframes fadein {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

/* Firefox < 16 */
@-moz-keyframes fadein {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

/* Safari, Chrome and Opera > 12.1 */
@-webkit-keyframes fadein {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

/* Internet Explorer */
@-ms-keyframes fadein {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

/* Opera < 12.1 */
@-o-keyframes fadein {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
</style>
