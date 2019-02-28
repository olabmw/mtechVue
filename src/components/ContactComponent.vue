<template>
  <v-container>
       <v-layout>
      <v-flex xs12 sm6 offset-sm3>
        <v-card>
          <v-img
            src="https://cdn.vuetifyjs.com/images/cards/desert.jpg"
            aspect-ratio="2.75"
          ></v-img>
  
          <v-card-title primary-title>
            <div>
              <h3 class="headline mb-0">{{name}}</h3>
              <div>Telefon: {{phone}}</div>
              <div>Mail: {{email}}</div>
            </div>
          </v-card-title>
  
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  props: ['name', 'phone', 'email']
}
</script>


<style>

</style>
