<template>
  <v-app-bar app class="appbar" color="#157ed2">
    <v-row class="" justify="center">
      <v-col cols="6"> </v-col>
      <v-col class="mb-7" cols="auto">
        <v-btn text color="white" x-small v-for="item in vbn" :key="item">
          <v-icon small>{{ item.icon }}</v-icon>
          {{ item.text }}
        </v-btn>
      </v-col>
    </v-row>
    <template v-slot:extension>
      <v-row justify="center" class="mb-4">
        <v-col class="pt-1" cols="auto">
          <v-img contain width="50" src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"></v-img>
        </v-col>
        <v-col class="px-0 pl-lg-2" :lg="5" cols="6">
          <v-text-field class="" flat clear-icon="mdi-close-circle" clearable hide-details label="Search" prepend-inner-icon="mdi-shopping-outline" solo>
            <template v-slot:append>
              <v-btn color="#157ed2" icon>
                <v-icon>
                  mdi-magnify
                </v-icon>
              </v-btn>
            </template></v-text-field
          >
        </v-col>
        <v-col class="mt-1" cols="auto">
          <v-menu open-on-hover offset-y nudge-bottom="5">
            <template v-slot:activator="{ on, attrs }">
              <v-btn v-bind="attrs" v-on="on">
                <span class="hidden-sm-and-down">我的购物车</span>
                <v-badge content="0" value="10" color="green" overlap>
                  <v-icon>
                    mdi-cart
                  </v-icon>
                </v-badge>
              </v-btn>
            </template>

            <v-list>
              <v-list-item>
                <v-list-item-title>123</v-list-item-title>
              </v-list-item>
              <v-list-item>
                <v-list-item-title>123</v-list-item-title>
              </v-list-item>
              <v-list-item>
                <v-list-item-title>123</v-list-item-title>
              </v-list-item>
              <v-list-item>
                <v-list-item-title>123</v-list-item-title>
              </v-list-item>
            </v-list>
          </v-menu>
        </v-col>
      </v-row>
    </template>
  </v-app-bar>
</template>
<script>
  export default {
    name: "AppBar",
    data: () => ({
      vbn: [
        { text: "我的账户", icon: "mdi-account" },
        { text: "愿望单", icon: "mdi-heart" },
        { text: "支持", icon: "mdi-help-circle" },
        { text: "登录", icon: "mdi-login-variant" },
        { text: "注册", icon: "mdi-arrow-up-box" },
      ],
    }),
  };
</script>
