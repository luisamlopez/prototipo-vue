<template>
  <div class="product-card">
    <img
      src="https://images.pexels.com/photos/276517/pexels-photo-276517.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940"
      alt=""
    />
    <div class="product-info">
      <div>
        <p><slot name="name"></slot></p>
        <p>$<slot name="price"></slot></p>
        <p>Stock: <slot name="stock"></slot> unidades</p>
      </div>
    </div>
  </div>
</template>

<style>
.product-card {
  width: 240px;
  box-shadow: 2px 2px 2px 1px var(--box-shadow);
  border-radius: 4px;
  border: 2px solid var(--vt-c-divider-dark-1);
}

.product-card img {
  width: 236px;
  height: 236px;
  border-radius: 4px;
  object-fit: cover;
}

.product-info {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 8px;
}

.product-info div p:nth-child(1) {
  font-weight: bold;
  font-size: var(--md);
}

.product-info figure {
  margin: 0;
}

.product-info figure img {
  width: 35px;
  height: 35px;
  margin-top: 0;
  margin-bottom: 4px;
}

.product-info div p:nth-child(2) {
  font-size: var(--sm);
  margin-top: 0;
  margin-bottom: 0;
  color: var(--very-light-pink);
}
</style>
