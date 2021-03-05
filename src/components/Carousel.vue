<template>
  <v-card tile>
    <v-carousel :show-arrows="false">
      <v-carousel-item v-for="(item, i) in i" :key="i" :src="i.src"></v-carousel-item>
    </v-carousel>
  </v-card>
</template>
<script>
  export default {
    name: "Carousel",
    data: () => ({}),
  };
</script>
