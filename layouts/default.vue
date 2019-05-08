<template>
  <div class="contain">
    <Nav />
    <nuxt />
    <Footer />
  </div>
</template>

<script>
import Nav from "~/components/Nav.vue"
import Footer from "~/components/Footer.vue"

export default {
  components: {
    Nav,
    Footer
  }
}
</script>

<style>
@import "../assets/styles/variables.css";
@import url("https://fonts.googleapis.com/css?family=Open+Sans:400,700");

html {
  font-family: "Open Sans", sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0 auto;
}

.contain {
  position: relative;
  margin: 0 auto;
  min-height: 100vh;
  height: 100%;
  padding-bottom: 50px;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
