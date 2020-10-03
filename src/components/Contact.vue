<template>
  <div id="ContactWrapper">
    <div id="LeftWrapper">
      <div id="LogoWrapper">
        <img src="../assets/logo_small.png" id="smallLogo" />
      </div>
    </div>
    <div id="RightWrapper"><p>This is the right wrapper</p></div>
  </div>
</template>

<script>
export default {
  name: "Contact",
};
</script>

<style lang="scss" scoped>
#ContactWrapper {
  width: 100%;
  display: inline-block;
  border: 2px green solid;
}
#LeftWrapper {
  width: 50%;
  height: 100%;
  border: 2px red solid;
  float: left;
}
#RightWrapper {
  width: 50%;
  border: 2px blue solid;
  float: left;
}

#smallLogo {
  width: 40px;
  height: 34px;
}
#LogoWrapper {
}
#ContactWrapper {
  padding-bottom: 3%;
  padding-top: 3%;
}
</style>
