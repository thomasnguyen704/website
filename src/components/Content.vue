<template>
  <article id="content">

    <b-container id="mission">
      <h2 class="font-weight-light">Plat is not just a financial management app, it’s also a way of living. At Plat we want you to live your best life and we know finances are part of that life. Plat helps you to budget without budgeting, we give without taking credit, and we guide you on your financial journey without interfering.</h2>
    </b-container>

    <div class="bg-light">
      <b-container id="howitworks">
        <b-row>
          <b-col sm="6">
            <p>Plat identifies your recurring bills and your income and disburses the average difference daily. </p> 
            <p>Plat, you know exactly how much you can spend each day to stay in the green! </p>
          </b-col>
          <b-col sm="6">
            <p>Behind the scenes, Plat is a debt product and simply by using the app you will build or repair your credit score!</p>
            <p>We partner with FDIC insured banks to ensure the safety and integrity of your relationship with Plat. Plat uses the latest security techniques to ensure that your data remains private.</p>
          </b-col>
        </b-row>
      </b-container>

      <b-container id="about">
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
              {{ card.title }} <br/>
              <a
                v-for="social in card.social"
                :key="social.url"
                :href="social.url"
              >
                <i :class="`mx-1 fa fa-${social.name}`"></i>
              </a>
            </b-card-text>
          </b-card>
        </b-card-group>
      </b-container>
    </div>
  </article>
</template>

<script>
export default {
  name: "Content",
  data() {
    return {
      cards: [
        {
          name: "Aaron Bridgers",
          pic: "aaron.jpg",
          title: "Founder",
          social: [
            {
              url: "https://www.linkedin.com/in/aaron-bridgers-cfa-frm-cia-512b8b9/",
              name: "linkedin",
            },
          ],
        },{
          name: "Chris Kennedy",
          pic: "chris.jpg",
          title: "Founder",
          social: [
            {
              url: "https://www.linkedin.com/in/christopherbkennedy/",
              name: "linkedin",
            },
          ],
        },{
          name: "Daniel Stahl",
          pic: "daniel.jpg",
          title: "Founder",
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
        },{
          name: "Thomas Nguyen",
          pic: "thomas.jpg",
          title: "Founder",
          social: [
            { 
              url: "https://www.linkedin.com/in/nguyentom/", 
              name: "linkedin" 
            },
          ],
        },
      ],
    };
  }
};
</script>

<style scoped>
#mission {
  padding-top: 10%;
  padding-bottom: 10%;
  text-align: center;
}
#howitworks,
#about {
  min-height: 80vh;
  padding-top: 10%;
  padding-bottom: 10%;
}
.margin {
  margin-right: 10px;
}
</style>