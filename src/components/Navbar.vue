<template>
  <div class="mynavbar">
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <img src="../assets/logo_large.png" width="178px" height="47px" />
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarColor03"
        aria-controls="navbarColor03"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div id="nav">
        <router-link to="/">Home</router-link> |
        <router-link to="/about">About</router-link>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>
.mynavbar {
  letter-spacing: 1px;
}
.navbar-collapse {
  margin-left: 80%;
}
</style>
