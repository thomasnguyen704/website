<template>
  <article id="content">
    <b-container id="section1" fluid>
      <b-container>
        <p class="display-4">We live to...</p>
        <p class="lead">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
          minim veniam, quis nostrud exercitation ullamco laboris nisi ut
          aliquip ex ea commodo consequat. Duis aute irure dolor in
          reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla
          pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
          culpa qui officia deserunt mollit anim id est laborum.
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
        <b-card-group deck>
          <b-card
            v-for="card in cards"
            :key="card.pic"
            :img-src="require(`../assets/${card.pic}`)"
            img-alt="..."
            img-top
            :title="card.name"
            title-tag="h5"
          >
            <b-card-text>
              {{ card.title }} <br />

              <a
                class="margin"
                v-for="social in card.social"
                :key="social.url"
                :href="social.url"
                ><i :class="`fa fa-${social.name}`"></i>
              </a>
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
      cards: [
        {
          name: "Daniel Stahl",
          pic: "profilepic.jpg",
          social: [
            {
              url: "https://github.com/danielhstahl",
              name: "github",
            },
            {
              url: "https://www.linkedin.com/in/daniel-stahl-6685a52a/",
              name: "linkedin",
            },
          ],
          title: "Founder",
        },
        {
          name: "Aaron Bridgers",
          pic: "aaron.jpeg",
          social: [
            {
              url:
                "https://www.linkedin.com/in/aaron-bridgers-cfa-frm-cia-512b8b9/",
              name: "linkedin",
            },
          ],
          title: "Founder",
        },
        {
          name: "Chris Kennedy",
          pic: "chris.jpeg",
          title: "Founder",
          social: [
            {
              url: "https://www.linkedin.com/in/christopherbkennedy/",
              name: "linkedin",
            },
          ],
        },
        {
          name: "Thomas Nguyen",
          pic: "thomas.jpeg",
          title: "Founder",
          social: [
            { url: "https://www.linkedin.com/in/nguyentom/", name: "linkedin" },
          ],
        },
      ],
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
.margin {
  margin-right: 10px;
}
</style>