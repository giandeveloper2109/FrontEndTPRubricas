<template>

    <v-responsive class="border pa-4">
      
    <div>
      <v-row>
 
        <v-col>
          <v-card text=" ">
            <v-container>
      <v-row>
        <v-card
    class="mx-auto my-8"
    max-width="344"
    elevation="16"
  >
    <v-card-item>
      <v-card-title>
        Edicion title
      </v-card-title>
      <v-card-subtitle>
        Card subtitle secondary text
      </v-card-subtitle>
    </v-card-item>

    <v-card-text>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    </v-card-text>
  </v-card>
      </v-row>
      <v-row>
        <v-card
    class="mx-auto my-8"
    max-width="344"
    elevation="16"
  >
    <v-card-item>
      <v-card-title>
        Card title
      </v-card-title>
      <v-card-subtitle>
        Card subtitle secondary text
      </v-card-subtitle>
    </v-card-item>

    <v-card-text>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    </v-card-text>
  </v-card>
      </v-row>






      
    </v-container>            
          </v-card >
        </v-col>
        <v-divider class="border-opacity-0" vertical></v-divider>
        <v-col>
    <v-card text="Contactenos" >
            <v-container>
      <v-row>
        <v-col
          cols="12"
          md="6"
        >
          <v-text-field
            v-model="firstname"
            :rules="nameRules"
            :counter="10"
            label="Nombre"
            required
            hide-details
          ></v-text-field>
        </v-col>



        <v-col
          cols="12"
          md="6"
        >
          <v-text-field
            v-model="email"
            :rules="emailRules"
            label="E-mail" 
            hide-details
            required
          ></v-text-field>
        </v-col>
      </v-row>
      <v-divider :thickness="20" class="border-opacity-0"></v-divider>
        <v-textarea label="Consulta"></v-textarea>
      
    </v-container>            
          </v-card>
        </v-col>
      </v-row>
    </div>
   

  </v-responsive>

</template>
<script>
  export default {
    data: () => ({
      valid: false,
      firstname: '',
      lastname: '',
      nameRules: [
        value => {
          if (value) return true

          return 'Name is required.'
        },
        value => {
          if (value?.length <= 10) return true

          return 'Name must be less than 10 characters.'
        },
      ],
      email: '',
      emailRules: [
        value => {
          if (value) return true

          return 'E-mail is requred.'
        },
        value => {
          if (/.+@.+\..+/.test(value)) return true

          return 'E-mail must be valid.'
        },
      ],
    }),
  }
</script>