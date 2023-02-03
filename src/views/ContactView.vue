<script setup>
import UserCard from "../components/UserCard.vue";
</script>

<template>
  <div class="contact">
    <div class="contact-header">
      <h1>¡Contáctame!</h1>
      <p>
        Si tienes alguna duda o quieres contactarme, puedes hacerlo a través de
        este formulario.
      </p>
      <img src="../assets/Luisa López.svg" alt="Contacto" />
    </div>
    <form @submit.prevent="submitForm" v-if="!formSubmitted">
      <div class="form__group">
        <span>Nombre completo</span>
        <input v-model="nombre" type="text" placeholder="Nombre completo" />
        <span>Email</span>
        <input v-model="email" type="email" placeholder="Email" />

        <span>Mensaje</span>
        <textarea v-model="mensaje" type="text" placeholder="Mensaje" />

        <span>Selecciona tus detalles favoritos:</span>
        <div class="check">
          <input
            type="checkbox"
            id="comp-inicio"
            value="Componentes del inicio"
            v-model="checkedNames"
          />
          <label for="comp-inicio">Componentes del inicio</label>
        </div>
        <div class="check">
          <input
            type="checkbox"
            id="inicio"
            value="Inicio"
            v-model="checkedNames"
          />
          <label for="inicio">Inicio</label>
        </div>
        <div class="check">
          <input
            type="checkbox"
            id="productos"
            value="Ejemplo de Inventario"
            v-model="checkedNames"
          />
          <label for="productos">Ejemplo de Inventario</label>
        </div>
      </div>
      <input class="submit" type="submit" value="Enviar" />
    </form>

    <div v-if="formSubmitted" class="card">
      <h2>¡Gracias por contactarme!</h2>
      <h3>Esta es solo una prueba para llamar a un componente</h3>
      <UserCard>
        <template #name>
          {{ nombre }}
        </template>
        <template #mail>
          {{ email }}
        </template>
        <template #msj>
          {{ mensaje }}
        </template>
        <template #detalles>
          {{
            checkedNames.length > 0
              ? checkedNames.join(", ")
              : "No seleccionaste ningún detalle."
          }}
        </template>
      </UserCard>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      nombre: "",
      email: "",
      mensaje: "",
      checkedNames: [],
      formSubmitted: false,
    };
  },
  methods: {
    submitForm: function () {
      this.formSubmitted = true;
    },
  },
};
</script>
<style>
form {
  display: flex;
  flex-direction: column;
  width: 100%;
  max-width: 500px;
  margin: 0 auto;
}
.contact-header {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 2rem;
}
.contact-header img {
  width: 100%;
  max-width: 300px;
}
input {
  padding: 4px 8px;
  margin: 4px;
}
.form__group {
  display: flex;
  flex-direction: column;
  margin-bottom: 1rem;
}

.form__group label {
  margin-bottom: 0.5rem;
}
span {
  font-size: 18px;

  font-weight: 500;
}
.form__group input,
.form__group textarea {
  padding: 0.5rem;
  border: 1px solid var(--vt-c-divider-dark-1);
  border-radius: 0.5rem;
  font-size: 1rem;
  transition: all 0.3s ease;
}
.submit {
  background-color: var(--vt-c-indigo);
  color: var(--vt-c-yellow);
  border: 0;
  padding: 0.5rem;
  font-size: 1.5rem;
  font-weight: 500;
  border-radius: 0.5rem;
  cursor: pointer;
  transition: all 0.3s ease;
}

.submit:hover {
  background-color: var(--vt-c-green);
  color: white;
}
.contact {
  padding: 2rem;
  justify-content: space-between;
}

.card {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
@media (min-width: 1024px) {
  .contact {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
  .contact-header {
    margin-bottom: 0;
  }
  .contact-header img {
    width: 100%;
    max-width: 500px;
  }
  .form {
    margin: 0;
  }
}
</style>
