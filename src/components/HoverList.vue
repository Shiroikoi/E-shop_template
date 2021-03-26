<template>
  <v-menu open-on-hover offset-x>
    <template v-slot:activator="{ on, attrs }">
      <v-list-item v-bind="attrs" v-on="on">
        <v-list-item-content>
          {{ categoryTitle }}
          <v-list-item-title>{{ title }}</v-list-item-title>
        </v-list-item-content>
        <v-list-item-icon><v-icon>mdi-chevron-right</v-icon></v-list-item-icon>
      </v-list-item>
    </template>
    <v-container>
      <v-row justify="center" v-for="row in rows" v-bind:key="row">
        <v-col v-for="col in row" cols="auto" v-bind:key="col">
          {{ col }}
        </v-col>
      </v-row>
    </v-container>
  </v-menu>
</template>
<script>
  export default {
    name: "HoverList",
    props: ["rows", "title", "categoryTitle"],
  };
</script>
