<template>
  <v-app class="grey lighten-5">
    <v-app-bar app><v-toolbar-title>Cart App</v-toolbar-title></v-app-bar>
    <v-container>
      <v-row>
        <v-col cols="12" sm="6" md="8">
          <Main />
        </v-col>
        <v-col cols="6" md="4">
          <Sidebar />
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
import Main from "./components/Main";
import Sidebar from "./components/Sidebar";
export default {
  name: "App",
  components: { Main, Sidebar },

  data: () => ({
    //
  }),
};
</script>
