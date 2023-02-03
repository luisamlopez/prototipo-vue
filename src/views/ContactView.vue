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

    <form class="form">
      <div class="form__group">
        <label for="name">Nombre</label>
        <input
          type="text"
          id="name"
          name="name"
          placeholder="Tu nombre"
          required
        />
        <label for="email">Correo electrónico</label>
        <input
          type="email"
          id="email"
          name="email"
          placeholder="Tu correo electrónico"
          required
        />

        <label for="message">Mensaje</label>
        <textarea
          id="message"
          name="message"
          placeholder="Escribe tu mensaje"
          required
        ></textarea>
      </div>

      <button type="submit" onclick="">Enviar</button>
    </form>
  </div>
</template>

<style>
.contact {
  padding: 2rem;
  justify-content: space-between;
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

.form {
  display: flex;
  flex-direction: column;
  width: 100%;
  max-width: 500px;
  margin: 0 auto;
}

.form__group {
  display: flex;
  flex-direction: column;
  margin-bottom: 1rem;
}

.form__group label {
  margin-bottom: 0.5rem;
}

.form__group input,
.form__group textarea {
  padding: 0.5rem;
  border: 1px solid var(--vt-c-divider-dark-1);
  border-radius: 0.5rem;
  font-size: 1rem;
  transition: all 0.3s ease;
}
button {
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

button:hover {
  background-color: var(--vt-c-green);
  color: white;
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

<script>
//función para enviar información del mensaje

export default {
  name: "ContactView",
};
</script>
