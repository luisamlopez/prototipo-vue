<script setup>
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
</script>

<template>
  <header>
    <div class="logos-collab">
      <img
        alt="Logo UDG"
        class="logo"
        src="http://www.udgvirtual.udg.mx/sites/default/files/logo_udgvirtual_marca_registrada_chico.jpg"
        width="300"
      />
      <span class="collab">En colaboración con </span>
      <img
        alt="Logo UCAB"
        class="logo"
        src="https://www.ucab.edu.ve/wp-content/uploads/2019/04/Logo_UCAB_1.png"
        width="300"
      />
    </div>

    <div class="wrapper">
      <HelloWorld msg="Prototipo para la Actividad 1.3" />
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
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

.logos-collab {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.collab {
  font-size: 1.5rem;
  font-weight: 500;
  margin: 1rem 0;
  text-align: center;
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
