<template>
  <v-sheet
    class="mx-auto my-4"
    max-width="1100"
  >
    <v-slide-group
      multiple
      show-arrows
      fade-transition
    >
      <v-slide-item
      v-for="photo in photos"
      :key="photo"
      class="ma-4"
      >
        <v-img
        :src="photo.src"
        width="300px"
        ></v-img>
      </v-slide-item>
    </v-slide-group>
  </v-sheet>
</template>

<script>
  export default {
    name: 'ProductSlide',

    data: () => ({
      photos: [
        {
          src: require('../assets/brownie1.jpeg'),
        },
        {
          src: require('../assets/brownie2.jpeg'),
        },
        {
          src: require('../assets/brownie3.jpeg'),
        },
        {
          src: require('../assets/brownie4.jpeg'),
        },
        {
          src: require('../assets/brownie5.jpeg'),
        },
        {
          src: require('../assets/brownie6.jpeg'),
        },
        {
          src: require('../assets/brownie7.jpeg'),
        },
      ],
    }),
  }
</script>
