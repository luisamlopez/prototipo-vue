<script setup>
import WelcomeItem from "./WelcomeItem.vue";
</script>

<template>
  <h5>
    Encuentra informaci贸n sobre esta colaboraci贸n internacional entre
    universidades. <br />馃憞馃憞馃徏馃憞馃徑馃憞馃徑馃憞馃従馃憞馃徔
  </h5>
  <ul>
    <li>
      <a href="https://www.udgvirtual.udg.mx/presentacion">UDG Virtual</a>
    </li>
    <li>
      <a href="https://www.ucab.edu.ve">Universidad Cat贸lica Andr茅s Bello</a>
    </li>
    <li>
      <a href="https://www.ucab.edu.ve/">Proyectos COIL</a>
    </li>
  </ul>
  <br />
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
    <template #msg>
      UDGVirtual es un 贸rgano desconcentrado de la Universidad de Guadalajara
      responsable de administrar y desarrollar programas acad茅micos de nivel
      medio superior y superior, en modalidades no escolarizadas, apoyadas en
      las tecnolog铆as de la informaci贸n y de la comunicaci贸n.</template
    >
  </WelcomeItem>

  <WelcomeItem>
    <template #imagen>
      <img
        src="https://www.ucab.edu.ve/wp-content/uploads/2019/04/Logo_UCAB_1.png"
        alt="Logo UCAB"
        style="width: 100%"
      />
    </template>
    <template #heading
      ><a class="heading" href="https://www.ucab.edu.ve/"
        >Universidad Cat贸lica Andr茅s Bello</a
      ></template
    >
    <template #msg>
      La Universidad Cat贸lica Andr茅s Bello, es una universidad privada con sede
      en Caracas, Venezuela, y con n煤cleos en Los Teques, Puerto Ordaz y Coro.
      Es miembro de la Asociaci贸n de Universidades Confiadas a la Compa帽铆a de
      Jes煤s en Am茅rica Latina, y la dirigen padres jesuitas.</template
    >
  </WelcomeItem>

  <WelcomeItem>
    <template #imagen>
      <img
        src="https://www.austral.edu.ar/comunicacion/wp-content/themes/uaunit/img/image.php?force=true&image=https://www.austral.edu.ar/comunicacion/wp-content/uploads/2019/11/coil-1.png&width=1000&height=292&cropratio=1000:292"
        alt="Logo Proyecto COIL"
        style="width: 90%"
      />
    </template>
    <template #heading
      ><a class="heading" href="https://www.ucab.edu.ve/"
        >Proyectos COIL</a
      ></template
    >
    <template #msg>
      La Coordinaci贸n de Proyectos COIL es la unidad funcional del Secretariado
      de Internacionalizaci贸n encargada de fomentar, facilitar y asesorar la
      realizaci贸n de proyectos de intercambio virtual colaborativo en l铆nea como
      estrategia fundamental del proceso de Internacionalizaci贸n en Casa de la
      UCAB.
    </template>
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
