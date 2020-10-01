<template>
  <div data-aos="flip-right" class="hello">
    <h1 id="msg">{{ msg }}</h1>
    <h3>99.4%</h3>
    <h5>
      of education institutions say that AI will be instrumental to their
      institution’s competitiveness.
    </h5>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/colors.scss";

#msg {
  color: #707070;
  font-family: "Brown Regular";
  font-weight: bold;
}

.hello {
  display: inline-block;
  width: 50%;
  padding: 7% 5%;
}

li {
  display: inline-block;
  margin: 0 10px;
}

h3 {
  color: $textcolor;
  display: inline-block;
  font-family: "Brown Regular";
}

h5 {
  color: $textcolor;
  display: inline-block;
  font-family: "Brown Regular";
}

@media only screen and (max-width: 965px) {
  h1 {
    font-size: 30px;
  }
  h5 {
    font-size: 14.25px;
  }
}

@media only screen and (max-width: 860px) {
  h1 {
    font-size: 25px;
  }
  h5 {
    font-size: 10px;
  }
}

@media only screen and (max-width: 607px) {
  h1 {
    font-size: 20px;
  }
  h5 {
    font-size: 8px;
  }
}
@media only screen and (max-width: 485px) {
  h1 {
    font-size: 15px;
  }
  h5 {
    font-size: 6px;
  }
}

@media only screen and (max-width: 365px) {
  h1 {
    font-size: 10px;
  }
  h5 {
    font-size: 4px;
  }
}
</style>
