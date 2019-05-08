<template>
  <div class="nav-wrapper">
    <div class="navbar">
      <a class="logo" href="/" title="Back to home" />
      <div class="nav-collapse">
        <ul class="nav-links">
          <li class="nav-link" title="Tutorials">
            Tutorials
          </li>
          <li class="nav-link" title="API">
            API
          </li>
          <li class="nav-link" title="Resources">
            Resources
          </li>
          <li class="nav-link" title="Plugins">
            Plugins
          </li>
          <li class="nav-link" title="Updates">
            Updates
          </li>
          <li class="nav-link" title="Help">
            Help
          </li>
        </ul>
      </div>
      <a href="javascript:void(0);" class="hamburger">
          <span class="hamburger-line hamburger-line-upper" />
          <span class="hamburger-line hamburger-line-middle" />
          <span class="hamburger-line hamburger-line-lower" />
      </a>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
@import "../assets/styles/variables.css";

.nav-wrapper {
  width: 100%;
}

.navbar {
  position: relative;
  margin: 0 auto;
  padding: 10px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  background: #fff;
}

.logo {
  background: url("/hapi.svg") no-repeat 0 0;
  background-size: contain;
  height: 75px;
  width: 100px;
  margin: 0;
}

.nav-collapse {
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
  box-sizing: border-box;
  border-radius: 6px;
  padding: 5px;
}

.nav-link:hover {
  color: #fff;
  background: var(--orange);
  transition: all 0.3s ease 0s;
}

.hamburger {
  position: absolute;
  display: none;
}

.hamburger-line {
  display: block;
  margin: 5px 0;
  width: 20px;
  height: 2px;
  border-radius: 5px;
  background: var(--black);
}

@media screen and (max-width: 900px){

  .navbar {
    position: fixed;
    top: 0;
    height: 50px;
    width: 100%;
    padding: 5px 0 0 0;
    border-bottom: 1px solid #ddd;
  }

  .logo {
    height: 50px;
    width: calc(100px * (2/3));
  }

  .nav-collapse {
    display: none;
  }

  .hamburger {
    display: inline-block;
    left: 20px;
    top: 12px;
  }
}
</style>
