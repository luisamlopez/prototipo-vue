<script setup>
import ProductCard from "../components/ProductCard.vue";
</script>

<template>
  <div>
    <h1>Ejemplo de componentes simulando inventario</h1>

    <div class="cards-container">
      <ProductCard>
        <template #name> Producto 1 </template>
        <template #price> 100 </template>
        <template #stock> 10 </template>
      </ProductCard>
      <ProductCard>
        <template #name> Producto 2 </template>
        <template #price> 200 </template>
        <template #stock> 20 </template>
      </ProductCard>
      <ProductCard>
        <template #name> Producto 3 </template>
        <template #price> 300 </template>
        <template #stock> 30 </template>
      </ProductCard>
      <ProductCard>
        <template #name> Producto 4 </template>
        <template #price> 400 </template>
        <template #stock> 40 </template>
      </ProductCard>
      <ProductCard>
        <template #name> Producto 5 </template>
        <template #price> 500 </template>
        <template #stock> 50 </template>
      </ProductCard>
      <ProductCard>
        <template #name> Producto 6 </template>
        <template #price> 600 </template>
        <template #stock> 60 </template>
      </ProductCard>
      <ProductCard>
        <template #name> Producto 7 </template>
        <template #price> 700 </template>
        <template #stock> 70 </template>
      </ProductCard>
      <ProductCard>
        <template #name> Producto 8 </template>
        <template #price> 800 </template>
        <template #stock> 80 </template>
      </ProductCard>
    </div>
  </div>
</template>

<style>
h1 {
  text-align: center;
  margin-bottom: 2rem;
}
.cards-container {
  display: grid;
  grid-template-columns: repeat(auto-fill, 240px);
  gap: 26px;
  place-content: center;
  margin: 0 auto;
  margin-bottom: 2rem;
}
@media (min-width: 1024px) {
  .code {
    display: flex;
    align-items: center;
  }
}
</style>
