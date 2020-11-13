<template>
  <v-app>
    <TopBar/>

    <v-main>
      <FirstPage/>
    </v-main>
  </v-app>
</template>

<script>
import FirstPage from './components/FirstPage';
import TopBar from './components/TopBar';

export default {
  name: 'App',

  components: {
    FirstPage,
    TopBar,
  },

  data: () => ({
    //
  }),
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Itim&display=swap');
</style>
