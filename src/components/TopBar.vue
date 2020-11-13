<template>
  <v-container>
    <v-app-bar
      app
      flat
      color="white"
      height="90px"
    >
    <v-row>

      <v-col class="categorias d-flex align-center justify-start">
          <v-btn text>sabores</v-btn>
          <v-btn text>novidades</v-btn>
          <v-btn text>kits</v-btn>
          <v-btn text>encomendas</v-btn>
      </v-col>

      <v-col class="d-flex justify-center">
        <v-img
          max-height="60"
          max-width="60"
          src="../assets/ELPIS_VAZADO.png"
        ></v-img>
      </v-col>

      <v-col class="d-flex align-center justify-end">
        <v-btn icon>
          <v-icon color="black">mdi-heart</v-icon>
        </v-btn>
        <v-btn icon>
          <v-icon color="black">mdi-magnify</v-icon>
        </v-btn>
      </v-col>

    </v-row>
    </v-app-bar>
  </v-container>
</template>

<script>
  export default {
    name: 'TopBar',

    data: () => ({}),
  }
</script>

<style>
  .categorias {
    font-family: 'Montserrat', sans-serif;
    font-weight: 100;
    font-size: 8px;
    justify-content: start;
    align-items: center;
    color: #67AFB9;
  }
</style>