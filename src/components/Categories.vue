<template>
  <v-card tile>
    <v-list dense>
      <v-list-group color="primary">
        <template v-slot:activator>
          <v-list-item>
            <v-list-item-content>
              CPU
            </v-list-item-content>
          </v-list-item>
        </template>
        <v-list-item-group>
          <v-menu open-on-hover offset-x>
            <template v-slot:activator="{ on, attrs }">
              <v-list-item v-bind="attrs" v-on="on">
                <v-list-item-title>AMD</v-list-item-title>
                <v-list-item-icon><v-icon>mdi-chevron-right</v-icon></v-list-item-icon>
              </v-list-item>
            </template>
            <v-container class="">
              <v-row>
                <v-col cols="auto">
                  1
                </v-col>
                <v-col cols="auto">
                  1
                </v-col>
                <v-col cols="auto">
                  1
                </v-col>
                <v-col cols="auto">
                  1
                </v-col>
              </v-row>
              <v-row>
                <v-col cols="auto">
                  1
                </v-col>
                <v-col cols="auto">
                  1
                </v-col>
                <v-col cols="auto">
                  1
                </v-col>
                <v-col cols="auto">
                  1
                </v-col>
              </v-row>
              <v-row>
                <v-col cols="auto">
                  1
                </v-col>
                <v-col cols="auto">
                  1
                </v-col>
                <v-col cols="auto">
                  1
                </v-col>
                <v-col cols="auto">
                  1
                </v-col>
              </v-row>
            </v-container>
          </v-menu>
          <v-menu open-on-hover offset-x>
            <template v-slot:activator="{ on, attrs }">
              <v-list-item v-bind="attrs" v-on="on">
                <v-list-item-title>Intel</v-list-item-title>
                <v-list-item-icon><v-icon>mdi-chevron-right</v-icon></v-list-item-icon>
              </v-list-item>
            </template>
            <v-row>
              <v-col cols="auto">
                1
              </v-col>
              <v-col cols="auto">
                1
              </v-col>
              <v-col cols="auto">
                1
              </v-col>
              <v-col cols="auto">
                1
              </v-col>
            </v-row>
            <v-row>
              <v-col cols="auto">
                1
              </v-col>
              <v-col cols="auto">
                1
              </v-col>
              <v-col cols="auto">
                1
              </v-col>
              <v-col cols="auto">
                1
              </v-col>
            </v-row>
            <v-row>
              <v-col cols="auto">
                1
              </v-col>
              <v-col cols="auto">
                1
              </v-col>
              <v-col cols="auto">
                1
              </v-col>
              <v-col cols="auto">
                1
              </v-col>
            </v-row>
          </v-menu>
        </v-list-item-group>
      </v-list-group>
    </v-list>
  </v-card>
</template>

<script>
  export default {
    name: "Categories",
  };
</script>
