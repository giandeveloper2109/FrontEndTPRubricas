<template>

    <v-responsive class="border pa-4">
      
    <div class="div-mod">
      <v-row class="custom-row">
 
        <v-col>
          <v-card class="custocard">
            <v-container class="custom-container">
      
      <v-row class="custom-row">
        <v-card
    class="mx-auto my-8"
    min-width="344"
    max-width="500"
    elevation="16"
    color="#26292F"
  >

    <v-card-item>
      <v-card-title style="margin-bottom: 5%;">
        Puede contactarnos por:
      </v-card-title>
      <v-card-subtitle class="custom-subtitle" style="font-size: 1.2rem; font-weight: bold;">
        Colaboraciones y Personalización
      </v-card-subtitle>
      <v-card-text class="custom-text">
        Si estás interesado en colaborar con nosotros en el desarrollo de nuevas 
        rubricas o necesitas adaptarlas a tus necesidades específicas, ¡contáctanos! 
        Estamos abiertos a personalizaciones y colaboraciones para mejorar nuestras 
        herramientas de evaluación
      </v-card-text>

      <v-card-subtitle class="custom-subtitle" style="font-size: 1.2rem; font-weight: bold;">
        Problemas Técnicos o Soporte
      </v-card-subtitle>

      <v-card-text class="custom-text">
        ¿Experimentando problemas técnicos o necesitas asistencia técnica? Háganoslo 
        saber y haremos nuestro mejor esfuerzo para resolver cualquier problema que 
        puedas tener con nuestras rubricas. Tu experiencia es importante para nosotros
      </v-card-text>

      <v-card-subtitle class="custom-subtitle" style="font-size: 1.2rem; font-weight: bold;">
        Feedback y Sugerencias
      </v-card-subtitle>

      <v-card-text class="custom-text">
        ¿Tienes ideas para mejorar nuestras rubricas o sugerencias para nuevos criterios? 
        Valoramos tu opinión y estamos interesados en recibir tu feedback. Juntos podemos 
        hacer que nuestras herramientas sean aún más efectivas
      </v-card-text>

      <v-card-subtitle class="custom-subtitle" style="font-size: 1.2rem; font-weight: bold;">
        Consultas Institucionales
      </v-card-subtitle>

      <v-card-text class="custom-text">
        Si representas a una institución educativa o a un grupo interesado en implementar 
        nuestras rubricas a nivel institucional, estamos aquí para discutir posibles 
        colaboraciones y proporcionarte la información que necesitas
      </v-card-text>
    </v-card-item>
    <v-card-text class="custom-text">
        ¡Estamos ansiosos por escucharte y trabajar juntos para mejorar la experiencia de evaluación!
      </v-card-text>
  </v-card>
      </v-row>
      





  
    </v-container>            
          </v-card >
        </v-col>
        <v-divider class="border-opacity-0" vertical></v-divider>
        <v-col class="custom-col">
    <v-card class="customcard" style="background-color: #26292F; color: #B0BAC5; margin-top: 3%;">
            <v-container>
              <!-- Poner aqui lo que haga falta -->
      <v-row>
        <v-col class="custom-col2"
          cols="12"
          md="6"
        >
          <v-text-field class="custom-input"
            v-model="firstname"
            :rules="nameRules"
            :counter="10"
            label="Nombre"
            required
            hide-details
          ></v-text-field>
          
        </v-col>

        <v-col class="custom-col2"
          cols="12"
          md="6"
        >
          <v-text-field class="custom-input"
            v-model="lastname"
            :rules="nameRules"
            :counter="10"
            label="Apellidos"
            required
            hide-details
          ></v-text-field>
          
        </v-col>


        <v-col
          cols="12"
          md="6"
        >
          <v-text-field class="custom-input"
            v-model="email"
            :rules="emailRules"
            label="E-mail" 
            hide-details
            required
          ></v-text-field>
        </v-col>
      </v-row>
      <v-divider :thickness="20" class="border-opacity-0"></v-divider>
        <v-textarea class="customtextarea" style="background-color: #434956; color: #B0BAC5;" label="Consulta"></v-textarea>
        <v-btn @click="submitForm" class="custobtn" >Enviar</v-btn>
    </v-container>            
          </v-card>
        </v-col>
      </v-row>

      

      
      
    </div>
   

  </v-responsive>

</template>



<style>
/* Agrega estilos personalizados en el bloque de estilo */

.custom-subtitle {
  color: #ECF9FB; /* Cambia el color del subtítulo a azul */
  font-family: 'Arial', sans-serif; /* Cambia la fuente del subtítulo */
  /* Otros estilos según tus necesidades */
  font-size: 1.5rem;
  font-weight: bold;
}

.custom-text {
  font-size: 1rem;;
  margin: 0px;
  height: none;
  min-height: none;
  max-height: none;
  color: #1BD96A;

}

.div-mod {
  background-color: #16181C;
  border: 0px;
}

.custom-row{
  background-color: #16181C;
  border: 0px;
}

.mx-auto {
  
}

.custom-container {
  background-color: purple;
  padding: 0px;
  margin: 0px;
}

.custom-col {
  background-color: #16181C;
}

.customcard {
  background-color: #16181C;
}

.custom-input {
  background-color: #434956;
}

.custom-input input:focus {
  border-color: #1BD96A; /* Cambia el color del borde al enfocar */
  box-shadow: 0 0 0 2px #1BD96A; /* Cambia el color del sombreado al enfocar */
}


.custom-col2 {
  background-color: #26292F;
}

.custobtn {
  margin-top: 5%;
  margin-left: 40%;
  width: 20%;
  background-color: #1BD96A;
}

.custocard {
  margin-top: 0px;
  padding: 0px;
  background-color: #26292F;
}

.customtextarea textarea:focus {
  border-color: #1BD96A !important; /* Cambia el color del borde al enfocar */
  box-shadow: 0 0 0 2px #1BD96A !important; /* Cambia el color del sombreado al enfocar */
}

</style>



<script>
export default {
  data: () => ({
    valid: false,
    firstname: '',
    lastname: '',
    nameRules: [
      value => {
        if (value) return true;

        return 'Name is required.';
      },
      value => {
        if (value?.length <= 10) return true;

        return 'Name must be less than 10 characters.';
      },
    ],
    email: '',
    emailRules: [
      value => {
        if (value) return true;

        return 'E-mail is requred.';
      },
      value => {
        if (/.+@.+\..+/.test(value)) return true;

        return 'E-mail must be valid.';
      },
    ],
  }),
  methods: {
    // Esta es la función para manejar el envío del formulario
    submitForm() {
      console.log('Formulario enviado:', {
        nombre: this.firstname,
        apellidos: this.lastname,
        correo: this.email,
        // Asegúrate de usar el nombre de propiedad correcto para la consulta
        consulta: this.message,
      });

      // Aquí puedes agregar la lógica para enviar la información del formulario al servidor
    },
  },
};
</script>
