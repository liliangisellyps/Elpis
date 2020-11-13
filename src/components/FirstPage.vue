<template>
  <v-container class="page">
    <h1 align="center" class="text">Conheça nossas delícias! <v-icon color="black">mdi-heart</v-icon></h1>
    <v-row>
    <ProductSlide/>
    </v-row>
    <h1 align="center" class="text">E aqui você encontra nosso cardápio:</h1>
    <v-row class="d-flex">
    <ProductCard/>
    </v-row>
    <v-row class="d-flex justify-center text">
      <v-text>Projeto desenvolvido para o Desafio PSEL Elpis Enactus UFAL <v-icon color="black" size="80%">mdi-heart</v-icon></v-text>
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

