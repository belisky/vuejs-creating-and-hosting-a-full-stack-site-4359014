<template>
  <div class="nav-bar">
    <div class="logo-wrap">
      <img :src="logo"/>
    </div>
    <button>Shopping cart</button>
  </div>

</template>

<script>
import logo from '@/assets/logo-hexagon.svg';
export default{
  name:"NavBar",
  data() {
    return {
      logo,
    }
  }
}
</script>