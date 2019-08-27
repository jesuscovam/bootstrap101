<template lang="html">
  <section class="bg-light">
    <b-container>
      <b-row>
        <b-col lg="6" order="2" order-lg="1" class="left">
          <h1>Bootstrap 101 template</h1>
          <p class="lead">Welcome text you'll be fine</p>
          <p>
            <a href="#" class="btn btn-primary">Discover more</a>
            <a href="#" class="btn btn-outline-primary">Some another action</a>
          </p>
        </b-col>
        <b-col lg="6" order="2" order-lg="1">
          <img src="../assets/macbook.png" alt="" class="img-fluid" />
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<script>
export default {};
</script>

<style lang="css" scoped>
.left {
  margin: auto
}
a {
  margin-left: 10px
}
</style>
