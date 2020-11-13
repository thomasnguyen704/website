<template>
  <b-jumbotron
    class="vertical-center jumbotron"
  >
    <video src="../assets/jumbo_video.mp4" autoplay loop playsinline muted></video>
    <template #header class='cursive'>Plat</template>

    <template #lead>
      Some subtitle
    </template>
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
.jumbotron {
  margin: 0px;
  border-radius: 0 !important;
  width: 100%;
  height: 100%;
  position: relative;
  overflow: hidden;
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
  z-index: 0;
}
.cursive {
  font-family: "Pacifico", cursive;
}
.vertical-center {
  min-height: 100%;
  min-height: 100vh;
  display: flex;
  align-items: center;
}
</style>