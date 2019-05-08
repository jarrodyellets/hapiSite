<template>
  <section class="container">
    <div class="index-header">
      <div class="index-header1">
        The Simple, Secure Framework
      </div>
      <div class="index-header2">
        Developers Trust
      </div>
    </div>
    <div class="index-description">
      Build
      <span class="bold">powerful</span>,
      <span class="bold">scalable applications</span>, with
      <span class="bold">minimal overhead</span> and full
      <span class="bold">out-of-the-box</span> functionality -
      <span class="bold">your code, your way</span>
    </div>
    <button class="index-button" href="/tutorials">
      Get started with hapi
    </button>
    <div class="index-footer">
      Originally developed to handle Walmart’s
      <span class="bold">Black Friday scale</span>, hapi continues to be the
      <span class="bold">proven</span> choice for
      <span class="bold">enterprise-grade</span> backend needs.
    </div>
  </section>
</template>

<script>
export default {
  components: {}
}

// let nav = document.querySelector('.navbar');
// let content = document.querySelector('.container');
// content.style.marginTop = nav.offsetHeight+'px';
</script>

<style>
@import "../assets/styles/variables.css";

.container {
  margin: 100px auto 0 auto;
  min-height: 100vh;
  max-width: 800px;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  color: var(--black);
}

.index-header {
  font-size: 2em;
  font-weight: 700;
}

.index-description {
  margin-top: 50px;
  font-size: 1.3em;
}

.index-button {
  border-radius: 10px;
  border: none;
  background: var(--orange);
  padding: 15px;
  font-size: 1.2em;
  font-weight: 700;
  margin: 40px 0;
  color: #fff;
  cursor: pointer;
  border: 4px solid rgba(0, 0, 0, 0);
}

.index-button:hover {
  border: 4px solid var(--orange);
  background: #fff;
  color: var(--orange);
  transition: all 0.3s ease 0s;
}

.index-footer {
  font-size: 1.3em;
}

.bold {
  font-weight: 700;
}
</style>
