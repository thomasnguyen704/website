<template>
  <b-jumbotron  id="jumbo" text-variant="white" fluid class="customjumbo" lead-tag="h2" header-tag="h1">
    <template #header ><h1 class="cursive display-1">Plat</h1></template>

    <template #lead >
      Some subtitle
    </template>
    <video src="../assets/jumbo_video.mp4" autoplay loop playsinline muted></video>
      
    <b-button variant="primary" href="#content">More</b-button>
  </b-jumbotron>
</template>

<script>
export default {
  name: "Jumbotron",
  /*props: {
    msg: String,
  },*/
};
</script>


<style scoped>
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
.container{
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