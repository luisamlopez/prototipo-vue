<template>
  <div class="item">
    <i>
      <slot name="imagen"></slot>
    </i>
    <div class="details">
      <h3>
        <slot name="heading"></slot>
      </h3>
      <p>
        <slot name="msg"></slot>
      </p>
    </div>
  </div>
</template>

<style scoped>
.item {
  margin-bottom: 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border: solid var(--color-border);
  border-radius: 4px;
  height: 280px;
  /* padding: 0.4rem 0 1rem calc(var(--section-gap) / 2); */
}

.details {
  flex: 1;
  padding: 10px;
}

.item i {
  display: flex;
  width: 50%;
  margin-top: 16px;
  place-self: center;
}

h3 {
  font-size: 1.2rem;
  font-weight: 500;
  margin-bottom: 0.4rem;
  color: var(--color-heading);
}

p {
  text-align: justify;
}
</style>
