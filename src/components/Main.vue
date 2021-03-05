<template>
  <v-main>
    <v-container fluid>
      <v-row justify="center">
        <v-col cols="2">
          <Categories />
        </v-col>
        <v-col cols="8">
          <Carousel />
        </v-col>
      </v-row>
    </v-container>
  </v-main>
</template>
<script>
  import Categories from "./Categories.vue";
  import Carousel from "./Carousel.vue";

  export default {
    name: "Main",
    components: {
      Categories,
      Carousel,
    },
    data: () => ({}),
  };
</script>
