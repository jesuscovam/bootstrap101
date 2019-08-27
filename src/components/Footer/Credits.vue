<template lang="html">
  <div class="py-3 bg-dark text-white">
    <b-container>
      <b-row>
        <b-col md="7" class="text-center text-md-left">
          <p class="mb-md-0">&copy; {{ date }} Jesus Cova</p>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  computed: {
    date() {
      const year = new Date();
      return year.getFullYear();
    }
  }
};
</script>

<style lang="css" scoped></style>
