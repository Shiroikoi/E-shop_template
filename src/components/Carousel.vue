<template>
  <v-card tile>
    <v-carousel cycle show-arrows-on-hover>
      <v-carousel-item :src="src"> </v-carousel-item>
    </v-carousel>
  </v-card>
</template>
<script>
  export default {
    name: "Carousel",
    data: () => ({
      src: require("../assets/i.jpg"),
      items: [
        {},
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/sky.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/bird.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/planet.jpg",
        },
      ],
    }),
  };
</script>
