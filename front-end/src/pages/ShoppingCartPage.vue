<template>
  <h1>Shopping Cart Page</h1>
  <div v-if="cartItems.length > 0">  
  <ShoppingCartList :cartItems="cartItems"/>
  </div>
  <div v-if="cartItems.length === 0">
      Your cart is empty
  </div>
</template>

<script>
import {cartItems} from '../temp-data';
import ShoppingCartList from '@/components/ShoppingCartList.vue';
export default {
  name: 'ShoppingCartPage',
  components:{
    ShoppingCartList,
  },
  data(){
    return {
      cartItems,
    }
  }
}
</script>