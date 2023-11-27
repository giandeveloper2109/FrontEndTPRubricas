<template>

    <v-footer
      class="bg-green-lighten-5 text-center d-flex flex-column"
    >

      <div>
        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4"
          :icon="icon"
          variant="text"
        ></v-btn>
      </div>
  
      <div class="pt-0">
        Aplicacion para la creacion de rubricas 
      </div>
  
      <v-divider></v-divider>
  
      <div>
        {{ new Date().getFullYear() }} — <strong>TP-GRUPO D&G </strong>
      </div>
    </v-footer>
  </template>
  <script>

import Formulario from './Formulario.vue';
  export default {
    data: () => ({
      
        icons: [
            "mdi-facebook",
            "mdi-twitter",
            "mdi-linkedin",
            "mdi-instagram",
        ],
    }),
    components: { Formulario }
}
</script>