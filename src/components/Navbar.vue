<template lang="html">
  <b-navbar toggleable="lg" type="light">
    <b-navbar-brand href="#">Bootstrap 101</b-navbar-brand>
    <b-navbar-toggle target="collapseMe"></b-navbar-toggle>
    <b-collapse id="collapseMe" is-nav>
      <b-navbar-nav class="ml-auto">
        <b-nav-item v-for="item in itemsList" :key="item.id">{{
          item
        }}</b-nav-item>
        <b-button size="md" variant="info">Sign in</b-button>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {
  data() {
    return {
      itemsList: ["About us", "Features", "Testimonials"]
    };
  }
};
</script>

<style lang="css" scoped></style>
