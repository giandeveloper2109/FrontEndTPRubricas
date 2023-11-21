<template >
  <div class="hero">

  <v-divider :thickness="20" class="border-opacity-0"></v-divider>
    <v-card
      class="mx-auto pa-12 pb-8"
      elevation="2"
      max-width="600"
      max-height="600"

    >
    <v-img
      class="mx-auto"
      max-width="150"
      src="../assets/logoD&G.png"
    ></v-img>
    <v-row>
      <v-col>
      <div class="text-subtitle-1 text-medium-emphasis">Nombres</div>
      <v-text-field
        density="compact"
        placeholder="Nombres del usuario"
        prepend-inner-icon="mdi-account-outline"
        variant="outlined"
      ></v-text-field>
      <div class="text-subtitle-1 text-medium-emphasis">Apellidos</div>
      <v-text-field
        density="compact"
        placeholder="Apellidos del usuario"
        prepend-inner-icon="mdi-account-outline"
        variant="outlined"
      ></v-text-field>
      <div class="text-subtitle-1 text-medium-emphasis">Usuario</div>
      <v-text-field
        density="compact"
        placeholder="Nombre del usuario"
        prepend-inner-icon="mdi-account-outline"
        variant="outlined"
      ></v-text-field>     
    </v-col>
    <v-col>
      <div class="text-subtitle-1 text-medium-emphasis">Celular</div>
      <v-text-field
        density="compact"
        placeholder="Numero de celular"
        prepend-inner-icon="mdi-phone-outline"
        variant="outlined"
      ></v-text-field>   
      <div class="text-subtitle-1 text-medium-emphasis">Correo</div>
      <v-text-field
        density="compact"
        placeholder="Email address"
        prepend-inner-icon="mdi-email-outline"
        variant="outlined"
      ></v-text-field>


      <div class="text-subtitle-1 text-medium-emphasis">Contraseña</div>  
      <v-text-field
        :append-inner-icon="visible ? 'mdi-eye-off' : 'mdi-eye'"
        :type="visible ? 'text' : 'password'"
        density="compact"
        placeholder="Enter your password"
        prepend-inner-icon="mdi-lock-outline"
        variant="outlined"
        @click:append-inner="visible = !visible"
      ></v-text-field>
    </v-col>
    </v-row>

      <v-btn
        block
        class="mb-8"
        color="green"
        size="large"
        variant="tonal"
      >
        Sign Up
      </v-btn>

    </v-card>
  </div>
</template>
<script>
export default {
  data: () => ({
    visible: false,
  }),
}
</script>
<style scoped>
.hero {
background: url('../assets/rubrica.jpg');
background-size: cover;
height: 100vh;
}
</style>