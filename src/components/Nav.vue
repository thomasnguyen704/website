<template>
  <b-navbar toggleable="lg" type="dark" variant="info">
    <b-navbar-brand href="#">Plat</b-navbar-brand>
    <b-navbar-toggle target="navbarSupportedContent"></b-navbar-toggle>
    <b-collapse id="navbarSupportedContent" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#">Link1</b-nav-item>
        <b-nav-item href="#">Link2</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {
  name: "Nav",
  /*props: {
    msg: String,
  },*/
};
</script>
<style scoped>
.navbar-brand {
  font-family: "Pacifico", cursive;
}
</style>