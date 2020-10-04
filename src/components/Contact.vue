<template>
  <div id="ContactWrapper" data-aos="fade-down">
    <div id="LeftWrapper">
      <div id="LogoWrapper">
        <img
          src="../assets/logo_small.png"
          id="smallLogo"
          style="float: left"
        />
        <p style="margin-left: 25%; font-size: 20px">SPIKY.AI</p>
        <br />
        <p>Izmir Bilimpark Teknokent</p>
        <p>
          Tekeli Fevzi Çakmak, 10032. Sk. No 2, 35865 ITOB Osb/Menderes/İzmir
        </p>
      </div>
    </div>
    <div id="RightWrapper">
      <div id="RightInLine">
        <p>For your questions:</p>
        <p style="color: #db4645; padding-left: 1em">info@spiky.ai</p>
      </div>
      <div id="RightInLine2">
        <p>Be a part of growing team:</p>
        <p style="color: #db4645; padding-left: 1em">info@spiky.ai</p>
      </div>
      <div id="SocialMedia">
        <img src="../assets/instagramMedium.png" />
        <img src="../assets/twitterMedium.png" />
        <img src="../assets/gmailMedium.png" />
        <img src="../assets/linkedinMedium.png" />
      </div>
    </div>
    <div id="GoogleMap">
      <p id="temp">TODO: ADD GOOGLE MAP LOCATION</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Contact",
};
</script>

<style lang="scss" scoped>
@import "../assets/colors.scss";

#ContactWrapper {
  width: 100%;
  display: inline-block;
  /*border: 2px green solid;*/
}
#LeftWrapper {
  width: 40%;
  height: 100%;
  /*border: 2px red solid;*/
  float: left;
}
#RightWrapper {
  width: 60%;
  /*border: 2px blue solid;*/

  margin: auto;
  overflow: hidden;
  display: inline-block;
  text-align: center;
}

#smallLogo {
  width: 40px;
  height: 34px;
}

#SocialMedia {
  /*display: ;border: 2px purple dotted;*/
  padding-top: 2%;
}

img {
  margin: 0% 3% 0% 3%;
}

#ContactWrapper {
  padding-bottom: 3%;
  padding-top: 3%;
}

#RightInLine2 {
  margin: 0% 5% 0% 5%;
  display: inline-block;
}

#RightInLine {
  margin: 0% 5% 0% 5%;
  display: inline-block;
}

p {
  font-family: "Brown Regular";
  color: $expcolor;
}

#GoogleMap {
  border: 2px red solid;
  margin-top: 5%;
  height: 75px;
}

#temp {
  vertical-align: middle;
  line-height: 75px;
  text-align: center;
}
</style>
