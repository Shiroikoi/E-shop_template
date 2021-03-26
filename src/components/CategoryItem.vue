<template>
  <v-list-group color="primary">
    <template v-slot:activator>
      <v-list-item>
        <v-list-item-content>
          {{ categoryTitle }}
        </v-list-item-content>
      </v-list-item>
    </template>
    <v-list-item-group>
      <slot> </slot>
    </v-list-item-group>
  </v-list-group>
</template>

<script>
  export default {
    name: "CategoryItem",
    props: ["categoryTitle"],
  };
</script>
