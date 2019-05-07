<template>
  <section class="container">
    <div class='index-header'>
      <div class='index-header1'>The Simple, Secure Framework</div>
      <div class='index-header2'>Develops Trust</div>
    </div>
    <div class='index-description'>Build <span class='bold'>powerful</span>, <span class='bold'>scalable applications</span>, with 
    <span class='bold'>minimal overhead</span> and full <span class='bold'>out-of-the-box</span> functionality - 
    <span class='underline'>your code, your way </span>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}

// let nav = document.querySelector('.navbar');
// let content = document.querySelector('.container');
// content.style.marginTop = nav.offsetHeight+'px';
</script>

<style>

.container {
  margin: 100px auto 0 auto;
  min-height: 100vh;
  max-width: 800px;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.index-header {
  font-size: 2em;
  font-weight: 700;
}

.index-description {
  margin-top: 50px;
  font-size: 1.5em;
}

.bold {
  font-weight: 700;
}

.underline {
  text-decoration: underline;
}
</style>
