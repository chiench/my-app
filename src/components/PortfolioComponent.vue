<template>
  <v-container class="mt-10">
   <v-row>
    <v-col  lg="12">
      <div style="text-align: center" >
      <h2 > About Us </h2>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ea, quam!</p>
      
        <v-btn :color="isActive === 'Web app'? 'success':'' " @click="isActive = 'Web app'"  rounded  elevation="2">Web App</v-btn>
        <v-btn :color="isActive === 'Mol app'? 'success':'' " @click="isActive ='Mol app'"  rounded  elevation="2">Mobile App</v-btn>
        <v-btn :color="isActive === 'Des app'? 'success':'' " @click="isActive ='Des app'"  rounded  elevation="2">Desktop App</v-btn>
      </div>
    </v-col>
   <slot v-if="isActive === 'Web app'">
      <v-col v-for="(card,index) in cards" :key="index" cols="3">
              <v-card>
                <v-img
                  :src="card.src"
                  class="white--text align-end"
                  gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                  height="200px"
                >
                  <v-card-title v-text="card.tilte">{{card.tilte}}</v-card-title>
                </v-img>
                  <v-spacer></v-spacer>
              </v-card>
            </v-col>
    </slot>
    <slot v-if="isActive === 'Des app'">
      <v-col v-for="(card,index) in cards2" :key="index" cols="3">
              <v-card>
                <v-img
                  :src="card.src"
                  class="white--text align-end"
                  gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                  height="200px"
                >
                  <v-card-title v-text="card.tilte">{{card.tilte}}</v-card-title>
                </v-img>
                  <v-spacer></v-spacer>
              </v-card>
            </v-col>
    </slot>
    <slot v-if="isActive === 'Mol app'">
      <v-col v-for="(card,index) in cards3" :key="index" cols="3">
              <v-card>
                <v-img
                  :src="card.src"
                  class="white--text align-end"
                  gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                  height="200px"
                >
                  <v-card-title v-text="card.tilte">{{card.tilte}}</v-card-title>
                </v-img>
                  <v-spacer></v-spacer>
              </v-card>
            </v-col>
    </slot>
    
      
    </v-row>
  </v-container>
</template>

<script>           

export default {
    data: () => ({
    isActive :'Web app',
    cards: [
      { tilte: "Web App 1", src: 'https://picsum.photos/id/11/500/300' },
      { tilte: "Web App 2", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Web App 2", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Web App 2", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Web App 3", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Web App 4", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Web App 5", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Web App 6", src: "https://picsum.photos/id/11/500/300" },
    ],
      cards2: [
      { tilte: "Des App 1", src: 'https://picsum.photos/id/11/500/300' },
      { tilte: "Des App 2", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Des App 2", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Des App 2", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Des App 3", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Des App 4", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Des App 5", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Des App 6", src: "https://picsum.photos/id/11/500/300" },
    ],
      cards3: [
      { tilte: "Mol App 1", src: 'https://picsum.photos/id/11/500/300' },
      { tilte: "Mol App 2", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Mol App 2", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Mol App 2", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Mol App 3", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Mol App 4", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Mol App 5", src: "https://picsum.photos/id/11/500/300" },
      { tilte: "Mol App 6", src: "https://picsum.photos/id/11/500/300" },
    ],
  }),
  methods: {
    change(){

    }
  }
};
</script>

<style>
</style>