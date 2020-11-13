<template>
  <v-container>
    <h1 align="center" class="text">Conheça nossas delícias!</h1>
    <v-row>
    <ProductSlide/>
    </v-row>
    <h1 align="center" class="text">E aqui você encontra nosso cardápio:</h1>
    <v-row class="d-flex">
    <ProductCard/>
    </v-row>
  </v-container>
</template>

<script>
import ProductCard from './ProductCard';
import ProductSlide from './ProductSlide';

export default {
  name: 'FirstPage',

  components: {
  ProductCard,
  ProductSlide,
},
  data: () => ({}),
}
</script>

<style>
  .text {
    font-family: 'Montserrat', sans-serif;
  }
</style>

