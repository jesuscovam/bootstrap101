<template lang="html">
  <div class="">
    <div class="py-5 bg-light">
      <b-container>
        <b-row class="rowText">
          <b-col lg="4" md="4" class="mb-lg-0">
            <h5>My bootstrap website</h5>
            <ul class="contact-info list-unstyled">
              <li>
                <a href="#">{{ email }}</a>
              </li>
              <li>
                <a href="#">+{{ tlf }}</a>
              </li>
            </ul>
            <p>Please write me on anything you're interested</p>
          </b-col>
          <b-col lg="4" md="6">
            <h5>Pages</h5>
            <ul
              v-for="page in pages"
              class="contact-info list-unstyled"
              :key="page.id"
            >
              <li>
                <a href="#">{{ page }}</a>
              </li>
            </ul>
          </b-col>
          <b-col lg="4" md="6">
            <h5>Links</h5>
            <ul
              v-for="data in favs"
              class="contact-info list-unstyled"
              :key="data.id"
            >
              <li>
                <a href="#">{{ data }}</a>
              </li>
            </ul>
          </b-col>
        </b-row>
        <b-row> </b-row>
      </b-container>
    </div>
    <Credits />
  </div>
</template>

<script>
import Credits from "./Credits";
export default {
  components: {
    Credits
  },
  data() {
    return {
      email: "jesuscovam@gmail.com",
      tlf: 5219841466416,
      pages: ["Twitter", "Facebook", "Instagram", "Youtube"],
      favs: ["Service to customer", "Taxi service", "Delivery"]
    };
  }
};
</script>

<style lang="css" scoped>
ul {
  list-style: none;
  text-align: left
}
h5{
  text-align: left
}
</style>
