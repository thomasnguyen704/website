<template>
<div id="top">
  <b-jumbotron
    id="jumbo"
    fluid
    class="customjumbo"
    lead-tag="h2"
    header-tag="h1"
  >
    <h1 class="cursive display-1">Plat</h1>
    <p class="lead">Everyday is Payday!</p>
    <video
      src="../assets/jumbo_video.mp4"
      autoplay
      loop
      playsinline
      muted 
    />
    <b-button variant="info" href="#content" class="mt-4">More</b-button>
  </b-jumbotron>
</div>
</template>

<script>
export default {
  name: "Jumbotron"
};
</script>


<style scoped>
h1 {
  color: orange;
}
#jumbo {
  margin: 0px;
  border-radius: 0 !important;
  width: 100%;
  height: 100%;
  position: relative;
  overflow: hidden;
  min-height: 100%;
  min-height: 100vh;
  display: flex;
  align-items: center;
}
.container {
  z-index: 1;
  text-align: center;
}
video {
  position: absolute;
  left: 50%;
  top: 50%;
  min-width: 100%;
  min-height: 100%;
  -webkit-transform: translate(-50%, -50%);
  -moz-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  z-index: -500;
}
.cursive {
  font-family: "Pacifico", cursive;
}
</style>