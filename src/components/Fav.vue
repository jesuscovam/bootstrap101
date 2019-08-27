<template lang="html">
  <b-container class="fav">
    <blockquote class="blockquote text-center mb-0">
      <svg class="lnr text-muted quote-icon pull-left">
        <use xlink:href="#lnr-heart"></use>
      </svg>
      <p class="mb-0">There is no website like this one</p>
      <footer class="blockquote-footer">
        Borito bebe in
        <cite title="Source Title">The House</cite>
      </footer>
    </blockquote>
  </b-container>
</template>

<script>
export default {};
</script>

<style lang="css" scoped>
.lnr {
  display: inline-block;
  fill: currentColor;
  width: 2em;
  height: 2em;
  vertical-align: -0.05em;
  stroke-width: 1;
}

.fav{
  margin-top: 40px
}
</style>
