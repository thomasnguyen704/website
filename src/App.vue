<template>
<div>
  <Nav />
  <Jumbotron />
  <Content />
  <Footer />
</div>
</template>

<script>
import Content from "./components/Content.vue";
import Footer from "./components/Footer.vue";
import Jumbotron from "./components/Jumbotron.vue";
import Nav from "./components/Nav.vue";

export default {
  name: "App",
  components: {
    Content,
    Footer,
    Jumbotron,
    Nav,
  },
};
</script>
<style>
body,
html {
  height: 100%;
  scroll-behavior: smooth;
}
</style>