<template>
  <v-container class="mt-3">
    <v-list class="tl-center">
      <v-subheader class="sub"> About Us </v-subheader>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ea, quam!</p>
      <v-list-item >
        <v-btn class="success" outlined elevation="2">Web App</v-btn>
        <v-btn outlined elevation="2">Mobile App</v-btn>
        <v-btn outlined elevation="2">Desktop App</v-btn>
      </v-list-item>
    </v-list>
    <v-row dense>
      <v-col v-for="(card,index) in cards" :key="index" cols="3">
        <v-card>
          <v-img
            :src="card.src"
            class="white--text align-end"
            gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
            height="200px"
          >
            <v-card-title v-text="card.title"></v-card-title>
          </v-img>
            <v-spacer></v-spacer>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>           

export default {
    data: () => ({
    cards: [
      { tilte: "Web App 1", img: "../assets/logo.png" },
      { tilte: "Web App 2", img: "../assets/logo.png" },
      { tilte: "Web App 3", img: "../assets/logo.png" },
      { tilte: "Web App 4", img: "../assets/logo.png" },
      { tilte: "Web App 5", img: "../assets/logo.png" },
    ],
  }),
};
</script>

<style>
</style>