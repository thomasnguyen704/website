<template>
  <article id="content">
    <b-container id="section1" fluid>
        <b-container >
            <p class="display-4">We live to...</p>
            <p class="lead">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
                tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim
                veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
                commodo consequat. Duis aute irure dolor in reprehenderit in voluptate
                velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint
                occaecat cupidatat non proident, sunt in culpa qui officia deserunt
                mollit anim id est laborum.
            </p>
        </b-container>
    </b-container>
    <b-container id="section2" class="bg-light" fluid>
        <b-container>
            <b-row>
                <b-col sm="6">Maybe an example from Kim</b-col>
                <b-col sm="6">Perhaps a technical explanation from the example</b-col>
            </b-row>
        </b-container>
    </b-container>
    <b-container id="section3" fluid>
        <b-container>
            <p class="display-4">About the Team</p>
            <b-card-group deck >
                <b-card v-for="card in cards" :key="card" img-src="../assets/placeholder.jpg" img-alt="..." img-top title="Person" title-tag="h5">
                    <b-card-text>
                        Title <br />
                        Socials
                    </b-card-text>
                </b-card>
            </b-card-group>
        </b-container>
    </b-container>
  </article>
</template>

<script>
export default {
  name: "Content",
  data() {
    return {
      cards: [0, 1, 2, 3],
    };
  },
  /*props: {
    msg: String,
  },*/
};
</script>

<style scoped>
#section1 {
  padding-top: 10%;
  padding-bottom: 10%;
  text-align: center;
}
#section2,
#section3 {
  min-height: 80vh;
  padding-top: 10%;
  padding-bottom: 10%;
}
</style>