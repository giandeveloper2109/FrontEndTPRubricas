<template>
    <v-responsive class="border pa-4">
    <div>
<v-row>
<v-col>
<!--Card 1-->     
    <v-card
      class="mx-auto"
      max-width="344"
    >
      <v-card-text>
        
        
        <p class="text-h4 text--primary">
          Definición y Propósito
        </p>
       
        <div class="text--primary">
          Una rúbrica es una herramienta de evaluación que establece criterios claros para la evaluación de tareas o proyectos.
           Su propósito principal es proporcionar una guía objetiva
           y transparente para la evaluación, facilitando la comprensión de las expectativas y mejorando la consistencia en la calificación."
        </div>
      </v-card-text>
      <v-card-actions>
        <v-btn
          variant="text"
          color="teal-accent-4"
          @click="reveal1 = true"
        >
          Learn More
        </v-btn>
      </v-card-actions>
  
      <v-expand-transition>
        <v-card
          v-if="reveal1"
          class="v-card--reveal"
          style="height: 100%;"
        >
          <v-card-text class="pb-0">
            <p class="text-h4 text--primary">
              ¿Cómo se diferencia de otros métodos de evaluación?
            </p>
            <p>A diferencia de métodos de evaluación más subjetivos, como las calificaciones tradicionales, las rúbricas ofrecen un enfoque más estructurado y objetivo para la evaluación. </p>
          </v-card-text>
          <v-card-actions class="pt-0">
            <v-btn
              variant="text"
              color="teal-accent-4"
              @click="reveal1 = false"
            >
              Close
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-expand-transition>
    </v-card>


    <v-divider :thickness="20" class="border-opacity-0"></v-divider>
<!--Card 2--> 
    <v-card
      class="mx-auto"
      max-width="344"
    >
      <v-card-text>
        
        <p class="text-h4 text--primary">
          Estructura y Componentes:

        </p>
        
        <div class="text--primary">
          La estructura típica de una rúbrica incluye criterios de evaluación específicos, niveles de desempeño y descripciones para cada nivel. 
          
        </div>
      </v-card-text>
      <v-card-actions>
        <v-btn
          variant="text"
          color="teal-accent-4"
          @click="reveal2 = true"
        >
          Learn More
        </v-btn>
      </v-card-actions>
  
      <v-expand-transition>
        <v-card
          v-if="reveal2"
          class="v-card--reveal"
          style="height: 100%;"
        >
          <v-card-text class="pb-0">
            <p class="text-h4 text--primary">
              ¿Cómo se organizan los criterios?
            </p>
            <p>  Los criterios se organizan jerárquicamente,con categorías principales y subcategorías que desglosan 
              los aspectos clave de la tarea.</p>
          </v-card-text>
          <v-card-actions class="pt-0">
            <v-btn
              variant="text"
              color="teal-accent-4"
              @click="reveal2 = false"
            >
              Close
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-expand-transition>
    </v-card>


</v-col>

<!--Divison de acerca de las rubricas--> 

<!--Divison de acerca de las rubricas-->    
<v-col>


<!--Card 3--> 
<v-card
      class="mx-auto"
      max-width="344"
    >
      <v-card-text>
        
        <p class="text-h4 text--primary">
          Cómo Crear y Utilizar Rúbricas
        </p>
        <p>adjective</p>
        <div class="text--primary">
          Para diseñar rúbricas efectivas, comienza identificando los criterios clave relacionados con la tarea. 
          Establece niveles de desempeño que reflejen la variación en la calidad del trabajo. 
          
        </div>
      </v-card-text>
      <v-card-actions>
        <v-btn
          variant="text"
          color="teal-accent-4"
          @click="reveal3 = true"
        >
          Learn More
        </v-btn>
      </v-card-actions>
  
      <v-expand-transition>
        <v-card
          v-if="reveal3"
          class="v-card--reveal"
          style="height: 100%;"
        >
          <v-card-text class="pb-0">
            <p class="text-h4 text--primary">
              ¿Cómo identificar criterios relevantes?
            </p>
            <p>Identificar criterios relevantes implica comprender los objetivos de la tarea y descomponerla en sus componentes fundamentales. </p>
          </v-card-text>
          <v-card-actions class="pt-0">
            <v-btn
              variant="text"
              color="teal-accent-4"
              @click="reveal3 = false"
            >
              Close
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-expand-transition>
    </v-card>


    


<!--Card 4--> 
    <v-card
      class="mx-auto"
      max-width="344"
    >
      <v-card-text>
       
        <p class="text-h4 text--primary">
          Beneficios y Mejores Prácticas
        </p>
        
        <div class="text--primary">
          Las rúbricas promueven la equidad, objetividad y claridad en la evaluación. Además, facilitan la retroalimentación constructiva
           y el desarrollo de habilidades. Para maximizar su efectividad, actualiza las rúbricas según sea necesario, comunica claramente los
            criterios a los evaluados. 
          
        </div>
      </v-card-text>
      <v-card-actions>
        <v-btn
          variant="text"
          color="teal-accent-4"
          @click="reveal4 = true"
        >
          Learn More
        </v-btn>
      </v-card-actions>
  
      <v-expand-transition>
        <v-card
          v-if="reveal4"
          class="v-card--reveal"
          style="height: 100%;"
        >
          <v-card-text class="pb-0">
            <p class="text-h4 text--primary">
              ¿Cómo las rúbricas aseguran consistencia en la evaluación?</p>
            <p>Al proporcionar criterios claros y descripciones detalladas para cada nivel de desempeño, las rúbricas reducen la ambigüedad y ayudan a los evaluadores a aplicar estándares consistentes, mejorando así la fiabilidad de la evaluación </p>
          </v-card-text>
          <v-card-actions class="pt-0">
            <v-btn
              variant="text"
              color="teal-accent-4"
              @click="reveal4 = false"
            >
              Close
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-expand-transition>
    </v-card>

   
</v-col>
</v-row>
</div>
</v-responsive>
  </template>
  <script>
  export default {
    data: () => ({
      reveal1: false,
      reveal2: false,
      reveal3: false,
      reveal4: false,
    }),
  }
</script>
<style>
.v-card--reveal {
  bottom: 0;
  opacity: 1 !important;
  position: absolute;
  width: 100%;
}
</style>