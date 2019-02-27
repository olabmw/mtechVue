<template>
  <v-app>
    <v-toolbar app style="background-color: #2C4870">
      <v-toolbar-title class="headline text-uppercase">
        <span style="color: white">MTECH</span>
        <!-- <span class="font-weight-light">MATERIAL DESIGN</span> -->
      </v-toolbar-title>
      <!-- <v-spacer></v-spacer> -->
      <!-- <v-btn
        flat
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
      >
        <span class="mr-2">Latest Release</span>
      </v-btn>-->
    </v-toolbar>

    <v-content style="background-color: white">

        <MainComponent/>
          <!-- TODO How to Send in details to the component -->
          <ContactComponent/>
          <ContactComponent/>

    </v-content>
  </v-app>
</template>

<script>
import MainComponent from "./components/MainComponent";
import ContactComponent from "./components/ContactComponent";

export default {
  name: "App",
  components: {
    MainComponent,
    ContactComponent
  },
  data() {
    return {
      //
    };
  }
};
</script>
