<template lang="html">
  <b-card
    :title="title"
    :img-src="imgCard"
    img-alt="image"
    img-top
    class="shadow border-0 h-100 inline-card"
  >
    <b-card-text>
      <p>{{ body }}</p>
      <a href="#">Read more</a>
    </b-card-text>
  </b-card>
</template>

<script>
export default {
  props: ["title", "body", "imgCard"]
};
</script>

<style lang="css" scoped></style>
