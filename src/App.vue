<script setup>
import { RouterLink, RouterView } from 'vue-router'
import FooterComponent from './components/FooterComponent.vue';
import SkillsComponent from './components/icons/SkillsComponent.vue';
</script>

<template>
  <head>
  <link rel="stylesheet" href="/Users/Ayann/Desktop/Intro to Responsive Webapps/Workshop 10/vue-project/src/styles.css">
</head>
  <div class="nav-container">
    <input type="checkbox" id="menu-toggle" class="menu-toggle" />
    <label for="menu-toggle" class="dropdown-btn">Menu</label>
    <div class="links-container">
      <RouterLink class="nav-link" to="/">Home</RouterLink>
      <RouterLink class="nav-link" to="/about">About</RouterLink>
      <RouterLink class="nav-link" to="/contact">Contact Me</RouterLink>
      <RouterLink class="nav-link" to="/check">Test Tab</RouterLink>
    </div>
  </div>


  <div class="page-container">
    <div class="content-wrapper">
      <RouterView />
      <SkillsComponent />
    </div>
    <footer class="amazing-footer">
      <FooterComponent />
    </footer>
  </div>
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
