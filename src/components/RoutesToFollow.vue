<script setup>
import WelcomeItem from "./WelcomeItem.vue";
</script>

<template>
  <h5>
    Encuentra información sobre esta colaboración internacional entre
    universidades. <br />👇👇🏼👇🏽👇🏽👇🏾👇🏿
  </h5>
  <WelcomeItem>
    <template #imagen>
      <img
        src="http://www.udgvirtual.udg.mx/sites/default/files/logo_udgvirtual_marca_registrada_chico.jpg"
        alt="Logo UDG"
        style="width: 100%"
      />
    </template>
    <template #heading
      ><a class="heading" href="https://www.udgvirtual.udg.mx/presentacion"
        >UDG Virtual</a
      ></template
    >

    UDGVirtual es un órgano desconcentrado de la Universidad de Guadalajara
    responsable de administrar y desarrollar programas académicos de nivel medio
    superior y superior, en modalidades no escolarizadas, apoyadas en las
    tecnologías de la información y de la comunicación.
  </WelcomeItem>

  <WelcomeItem>
    <template #imagen>
      <img
        src="https://www.ucab.edu.ve/wp-content/uploads/2019/04/Logo_UCAB_1.png"
        alt="Logo UCAB"
        style="width: 100%"
      />
    </template>
    <template #heading>Universidad Católica Andrés Bello</template>

    La Universidad Católica Andrés Bello, es una universidad privada con sede en
    Caracas, ​​​ Venezuela, y con núcleos en Los Teques, Puerto Ordaz y Coro. Es
    miembro de la Asociación de Universidades Confiadas a la Compañía de Jesús
    en América Latina, y la dirigen padres jesuitas
  </WelcomeItem>

  <WelcomeItem>
    <template #imagen>
      <img
        src="http://www.udgvirtual.udg.mx/sites/default/files/logo_udgvirtual_marca_registrada_chico.jpg"
        alt="Logo UDG"
        style="width: 100%"
      />
    </template>
    <template #heading>Documentation</template>

    Vue’s
    <a href="https://vuejs.org/" target="_blank" rel="noopener"
      >official documentation</a
    >
    provides you with all information you need to get started.
  </WelcomeItem>

  <WelcomeItem>
    <template #imagen>
      <img
        src="http://www.udgvirtual.udg.mx/sites/default/files/logo_udgvirtual_marca_registrada_chico.jpg"
        alt="Logo UDG"
        style="width: 100%"
      />
    </template>
    <template #heading> Documentation</template>

    Vue’s
    <a href="https://vuejs.org/" target="_blank" rel="noopener"
      >official documentation</a
    >
    provides you with all information you need to get started.
  </WelcomeItem>
</template>

<style>
h5 {
  margin-top: 10px;
  margin-bottom: 10px;
  color: #2c3e50;
  font-size: 18px;
  text-align: center;
}

.heading {
  color: var(--color-heading);
  font-size: 1.2rem;
  font-weight: 500;
  margin-bottom: 0.4rem;
}
</style>
