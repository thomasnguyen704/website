<template>
  <b-navbar toggleable="lg" type="dark" variant="dark" fixed="top">
    <b-navbar-brand href="#top" id="brand">
      <img
        src="../assets/plat_logo.png"
        class="d-inline-block align-top"
        alt="logo"
        width="30"
        height="30"
        alt-img="plat logo"
      />
    </b-navbar-brand>
    <b-navbar-toggle target="navbarSupportedContent"></b-navbar-toggle>
    <b-collapse id="navbarSupportedContent" is-nav>
      <b-navbar-nav class="mr-auto" small>
        <b-nav-item href="#mission">Mission</b-nav-item>
        <b-nav-item href="#howitworks">How it works</b-nav-item>
        <b-nav-item href="#about">About us</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {
  name: "Nav"
};
</script>

<style scoped>
#brand {
  font-family: "Pacifico", cursive;
}
</style>