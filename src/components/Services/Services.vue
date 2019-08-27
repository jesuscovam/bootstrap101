<template lang="html">
  <section>
    <b-container>
      <h2 class="title">Services</h2>
      <p class="text-muted mb-5">These are some examples of our treatment</p>
      <b-row>
        <b-col sm="6" lg="4" class="mb-3" v-for="icon in icons" :key="icon.id">
          <Service :iconSvg="icon.icon" :title="icon.title" :body="icon.body" />
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
import Service from "./Service";
export default {
  data() {
    return {
      icons: [
        {
          icon: "lnr-magic-wand",
          title: "This is the connection",
          body: "detailed info"
        },
        {
          icon: "lnr-heart",
          title: "This is the connection",
          body: "detailed info"
        },
        {
          icon: "lnr-rocket",
          title: "This is the connection",
          body: "detailed info"
        },
        {
          icon: "lnr-paperclip",
          title: "This is the connection",
          body: "detailed info"
        },
        {
          icon: "lnr-screen",
          title: "This is the connection",
          body: "detailed info"
        },
        {
          icon: "lnr-inbox",
          title: "This is the connection",
          body: "detailed info"
        }
      ]
    };
  },
  components: {
    Service
  }
};
</script>

<style lang="css" scoped>
section{
  text-align: left
}
.title {
  margin-top: 20px
}
</style>
