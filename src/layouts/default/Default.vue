<template>
  <v-app>
    
    <default-bar />

    <default-view />
    <Formulario/>
    <FooterView/>
  </v-app>
</template>

<script setup>
  import DefaultBar from './AppBar.vue'
  import DefaultView from './View.vue'
  import FooterView from '@/components/Footer.vue'
  import Formulario from '@/components/Formulario.vue';
  import Carrusel from '@/components/Carrusel.vue';
</script>
