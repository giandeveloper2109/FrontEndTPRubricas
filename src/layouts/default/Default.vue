<template>
  <v-app>
    
    <default-bar />

    <default-view />
    <div>
      <v-sheet class="bg-green-lighten-5 text-center d-flex flex-column">
			  <h1 >Acerca de nosotros</h1>
        
		  </v-sheet>
    </div>
    <Aboutus/>
    <div>
      <v-sheet class="bg-green-lighten-5 text-center d-flex flex-column">
			  <h1 >RUBRICAS</h1>
        
		  </v-sheet>
    </div>
    <AcercaDerRUBRICAS/>
    <div>
      <v-sheet class="bg-green-lighten-5 text-center d-flex flex-column">
			  <h1 >Contactenos</h1>
        
		  </v-sheet>
    </div>
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
  import Aboutus from '@/components/Aboutus.vue';
  import AcercaDerRUBRICAS from '@/components/AcercaDerRUBRICAS.vue';
</script>
<style>
h1 { color: #00bf63; }
</style>