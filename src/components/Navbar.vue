<template>
  <div class="mynavbar">
    <b-navbar toggleable="lg" type="faded" variant="light">
      <b-navbar-brand href="#">
        <img
          src="../assets/logo_large.png"
          width="178px"
          height="47px"
          class="d-inline-block align-top"
          alt="Kitten"
        />
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <div id="nav">
            <router-link to="/">Home</router-link> |
            <router-link to="/about">About</router-link>
          </div>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>
.mynavbar {
  /*position: fixed; */
  width: 100vw; /* take up the full browser width */
  z-index: 200; /* high z index so other content scrolls underneath */
  letter-spacing: 1px;
  padding: 0% 15%;
}

@media only screen and (max-width: 760px) {
  img {
    width: 125px;
    height: 35px;
  }
}

@media only screen and (max-width: 560px) {
  img {
    width: 89px;
    height: 24px;
  }
}

@media only screen and (max-width: 485px) {
  img {
    width: 60px;
    height: 16px;
  }
}
</style>
