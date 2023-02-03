<template>
  <div class="item">
    <h3>Nombre:</h3>
    <p><slot name="name"></slot></p>
    <h3>Email:</h3>
    <p><slot name="mail"></slot></p>
    <h3>Mensaje:</h3>
    <p><slot name="msj" class="msj"></slot></p>
  </div>
</template>

<style scoped>
.item {
  margin: 0;
  display: flex;
  flex-direction: column;
  align-items: left;
  justify-content: left;
  border: solid var(--color-border);
  border-radius: 4px;
  height: 250px;
  width: 250px;
  padding: 0.5rem;
}
h3 {
  font-size: 1.2rem;
  font-weight: 500;
  color: var(--color-heading);
}

p {
  margin: 0;
  padding: 0;
  overflow: hidden;
}
</style>
