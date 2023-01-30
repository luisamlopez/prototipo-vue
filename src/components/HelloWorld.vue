<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <div class="greetings">
    <h1 class="titulo">{{ msg }}</h1>
    <h3>
      La presente es una actividad evaluativa diseño y maquetado libre,
      utilizando los componentes, rutas y navegación propios del Framework
      Vue.js.
    </h3>
    <h4>
      Realizado por: <a href="https://github.com/luisamlopez">Luisa López</a>
    </h4>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

h4 {
  margin-top: 1.5rem;
  font-size: 1rem;
  text-align: center;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
