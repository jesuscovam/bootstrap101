<template lang="html">
  <section class="bg-light">
    <b-container>
      <h2>Portfolio</h2>
      <p class="lead text-muted mb-5">Our craft</p>
      <b-row>
        <b-col v-for="card in cards1" :key="card.id">
          <Card
            :title="card.title"
            :imgCard="card.img"
            :body="card.body"
            :key="card.id"
          />
        </b-col>
      </b-row>
      <b-row class="row2">
        <b-col v-for="card in cards2" :key="card.id">
          <Card
            :title="card.title"
            :imgCard="card.img"
            :body="card.body"
            :key="card.id"
          />
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
import Card from "./Card";
export default {
  components: {
    Card
  },
  data() {
    return {
      cards1: [
        {
          img: require("../../assets/mockup0.jpg"),
          title: "Services to Ipanema",
          body: "They were looking for a tropical vibe"
        },
        {
          img: require("../../assets/mockup1.jpg"),
          title: "Services to Ipanema",
          body: "They were looking for a tropical vibe"
        },
        {
          img: require("../../assets/mockup2.jpg"),
          title: "Services to Ipanema",
          body: "They were looking for a tropical vibe"
        }
      ],
      cards2: [
        {
          img: require("../../assets/mockup3.jpg"),
          title: "Services to Ipanema",
          body: "They were looking for a tropical vibe"
        },
        {
          img: require("../../assets/mockup4.jpg"),
          title: "Services to Ipanema",
          body: "They were looking for a tropical vibe"
        },
        {
          img: require("../../assets/mockup6.jpg"),
          title: "Services to Ipanema",
          body: "They were looking for a tropical vibe"
        }
      ]
    };
  }
};
</script>

<style lang="css" scoped>
.row2{
  margin-top: 20px
}
</style>
