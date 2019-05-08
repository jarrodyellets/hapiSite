<template>
  <nav role="navigation" class="navbar">
    <a class="logo" href="/" title="Back to home"/>
    <div class="nav-collapse">
      <ul class="nav-links">
        <li class="nav-links-li">
          <a class="nav-link" title="Tutorials" href="/tutorials">Tutorials</a>
        </li>
        <li class="nav-links-li">
          <a class="nav-link" title="API" href="/api">API</a>
        </li>
        <li class="nav-links-li">
          <a class="nav-link" title="Resources" href="/resources">Resources</a>
        </li>
        <li class="nav-links-li">
          <a class="nav-link" title="Plugins" href="/plugins">Plugins</a>
        </li>
        <li class="nav-links-li">
          <a class="nav-link" title="Updates" href="/updates">Updates</a>
        </li>
        <li class="nav-links-li">
          <a class="nav-link" title="Help" href="/help">Help</a>
        </li>
      </ul>
    </div>
    <a href="javascript:void(0);" class="hamburger">
      <span class="hamburger-line hamburger-line-upper"/>
      <span class="hamburger-line hamburger-line-middle"/>
      <span class="hamburger-line hamburger-line-lower"/>
    </a>
  </nav>
</template>

<script>
export default {};
</script>

<style>
@import "../assets/styles/variables.css";

.navbar {
  position: relative;
  width: 100%;
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

.nav-links-li {
  display: inline-block;
}

.nav-link {
  position: relative;
  margin: 10px;
  cursor: pointer;
  color: var(--orange);
  font-weight: 700;
  box-sizing: border-box;
  border-radius: 6px;
  padding: 5px;
  text-decoration: none;
}

.nav-link:before{
  width: 0;
  position: absolute;
  content: "";
  left: 0;
  top: 0;
  height: 2px;
  background: var(--orange);
}

.nav-link:after {
  width: 0;
  position: absolute;
  content: "";
  right: 0;
  top: 0;
  height: 2px;
  background: var(--orange);
}

.nav-link:hover:before {
  width: 50%;
  -webkit-transition: width 2s ease-in;
  transition: width .2s ease-in;
}

.nav-link:hover:after, .nav-link:hover:before {
  width: 50%;
  -webkit-transition: width 2s ease-in;
  transition: width .2s ease-in;
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

@media screen and (max-width: 900px) {
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
    width: calc(100px * (2 / 3));
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
