<template>
  <div class="nav-wrapper">
    <div class="navbar">
      <a class="logo" href="/" title="Back to home"/>
      <ul class="nav-links">
        <li class="nav-link" title="Tutorials">Tutorials</li>
        <li class="nav-link" title="API">API</li>
        <li class="nav-link" title="Plugins">Plugins</li>
        <li class="nav-link" title="Updates">Updates</li>
        <li class="nav-link" title="Contribute">Contrubute</li>
        <li class="nav-link" title="Resources">Resources</li>
        <li class="nav-link" title="Help">Help</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
@import "../assets/styles/variables.css";

.nav-wrapper {
  position: fixed;
  top: 0;
  width: 100%;
  max-width: 1260px;
  margin: 0 auto;
}

.navbar {
  padding: 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  background: url("../static/hapi.svg") no-repeat 0 0;
  background-size: contain;
  height: 75px;
  width: 100px;
  margin: 0;
}

.nav-links {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.nav-link {
  display: inline-block;
  margin: 10px;
  cursor: pointer;
  color: var(--orange);
  font-weight: 700;
}
</style>
