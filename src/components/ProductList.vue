<template>
  <ul class="catalog__list">
    <ProductItem
      :product="product"
      v-for="(product, index) in products"
      v-bind:key="index"
    ></ProductItem>
  </ul>
</template>

<script>
import ProductItem from "./ProductItem.vue";
export default {
  props: ["products"],
  components: { ProductItem },
};
</script>
