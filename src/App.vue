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
      <div v-for="contact in contacts" :key="contact.phone">
        <ContactComponent v-bind:name="contact.name" v-bind:phone="contact.phone" v-bind:email="contact.email"/>
      </div>
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
      contacts: [
        {
          name: "Namn1",
          phone: "12342345345",
          email: "jag@hemma1"
        },
        {
          name: "Namn2",
          phone: "7546523",
          email: "jag@hemma2"
        }
      ]
    };
  }
};
</script>

<style>

</style>

