<template>
  <v-app-bar  color="transparent">
    <v-img
        src="../assets/logoD&G.png"
      ></v-img>
    <v-app-bar-title >

      D&G-Rubrics
    </v-app-bar-title>
    <v-spacer></v-spacer>
    <v-btn plain>Home</v-btn>
    <v-btn plain>Quienes Somos</v-btn>
    <v-btn plain>Rubricas</v-btn>
    <v-btn plain>Premiun</v-btn>
    <v-btn plain>Contactenos</v-btn>
    <v-btn  variant="plain" to="/Login" >Login</v-btn>
    
    <v-btn variant="tonal" router-link to="/registrarse">Sign Up</v-btn>

    
  </v-app-bar>
</template>

<script setup>
  //
</script>
