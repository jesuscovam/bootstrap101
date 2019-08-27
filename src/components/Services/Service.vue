<template lang="html">
  <div class="">
    <svg class="lnr text-primary services-icon">
      <use v-bind="{ 'xlink:href': `#${iconSvg}` }"></use>
    </svg>
    <p>
      <strong>{{ title }}</strong>
    </p>
    <p>{{ body }}</p>
  </div>
</template>

<script>
export default {
  props: ["iconSvg", "title", "body"]
};
</script>

<style lang="css" scoped>

.lnr {
  display: inline-block;
  fill: currentColor;
  width: 1em;
  height: 1em;
  vertical-align: -0.05em;
  stroke-width: 1;
}

.services-icon {
  margin-bottom: 20px;
  font-size: 30px;
}
</style>
