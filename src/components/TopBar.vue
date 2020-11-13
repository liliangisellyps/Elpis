<template>
  <v-container>
    <v-app-bar
      app
      flat
      color="white"
      height="90px"
    >
    <v-row>

      <v-col class="categorias d-flex">
          <v-btn text color="#8a191d">sabores</v-btn>
          <v-btn text color="#8a191d">novidades</v-btn>
          <v-btn text color="#8a191d">kits</v-btn>
          <v-btn text color="#8a191d">encomendas</v-btn>
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
        <v-icon color="#8a191d">mdi-heart</v-icon>
        </v-btn>

        <v-btn icon>
          <v-icon color="#8a191d">mdi-magnify</v-icon>
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
    font-family: 'Itim', cursive;
    font-weight: 100;
    font-size: 8px;
    justify-content: start;
    align-items: center;
  }
</style>