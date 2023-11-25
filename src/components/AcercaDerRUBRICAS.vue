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
        <div>Word of the Day</div>
        <p class="text-h4 text--primary">
          el·ee·mos·y·nar·y
        </p>
        <p>adjective</p>
        <div class="text--primary">
          relating to or dependent on charity; charitable; charitable donations. Pertaining to alms.<br>
          "an eleemosynary educational institution."
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
              Origin
            </p>
            <p>late 16th century (as a noun denoting a place where alms were distributed): from medieval Latin eleemosynarius, from late Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’ </p>
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
        <div>Word of the Day</div>
        <p class="text-h4 text--primary">
          el·ee·mos·y·nar·y
        </p>
        <p>adjective</p>
        <div class="text--primary">
          relating to or dependent on charity; charitable; charitable donations. Pertaining to alms.<br>
          "an eleemosynary educational institution."
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
              Origin
            </p>
            <p>late 16th century (as a noun denoting a place where alms were distributed): from medieval Latin eleemosynarius, from late Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’ </p>
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
        <div>Word of the Day</div>
        <p class="text-h4 text--primary">
          el·ee·mos·y·nar·y
        </p>
        <p>adjective</p>
        <div class="text--primary">
          relating to or dependent on charity; charitable; charitable donations. Pertaining to alms.<br>
          "an eleemosynary educational institution."
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
              Origin
            </p>
            <p>late 16th century (as a noun denoting a place where alms were distributed): from medieval Latin eleemosynarius, from late Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’ </p>
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
        <div>Word of the Day</div>
        <p class="text-h4 text--primary">
          el·ee·mos·y·nar·y
        </p>
        <p>adjective</p>
        <div class="text--primary">
          relating to or dependent on charity; charitable; charitable donations. Pertaining to alms.<br>
          "an eleemosynary educational institution."
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
              Origin
            </p>
            <p>late 16th century (as a noun denoting a place where alms were distributed): from medieval Latin eleemosynarius, from late Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’ </p>
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