<template>
  <div class="product-container" v-for="product in cartItems" :key="product.id">
    <img :src="product.imageUrl" class="product-image" />
    <div class="details-wrap">
      <h3>{{ product.name }}</h3>
      <p>{{ product.price }}</p>
    </div>
    <button class="remove-button">Remove from Cart</button>
  </div>
  <button class="checkout-button">Proceed to Checkout</button>
</template>

<script>
export default {
  name: "ShoppingCartList",
  props: ["cartItems"],
};
</script>
