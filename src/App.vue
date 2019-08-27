<template>
  <div id="app">
    <Navbar />
    <Hero />
    <Services />
    <Portfolio />
    <Fav />
    <Footer />
  </div>
</template>

<script>
import Navbar from "./components/Navbar";
import Hero from "./components/Hero";
import Services from "./components/Services/Services";
import Portfolio from "./components/Portfolio/Portfolio";
import Fav from "./components/Fav";
import Footer from "./components/Footer/Footer";

export default {
  name: "app",
  components: {
    Navbar,
    Hero,
    Services,
    Portfolio,
    Fav,
    Footer
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
