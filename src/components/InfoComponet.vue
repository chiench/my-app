<template>
  <v-container class="mt-20">
    <v-row>
      <v-col lg="6">
        <h1>Welcome to my web</h1>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sed nesciunt
          alias laudantium accusamus, quae ipsam ut quibusdam omnis cupiditate
          molestias.
        </p>

        <v-btn :loading="loading" class="mr-4" color="success" rounded @click="change()"
          >Get Started</v-btn
        >
        <v-btn color="primary" rounded>
          <v-icon class="mr-2">mdi-play-circle-outline</v-icon> Watch</v-btn
        >
      </v-col>
      <v-col lg="6">
        <img src="../assets/logo.png" width="100%" alt="" />
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () =>{
    return {
      loading: false,
    }
  },
  methods: {
    change(){
      this.loading = true
      setTimeout(() => {
        this.loading = false
      }, 3000);
    }
  }
};
</script>

<style scoped>
h1 {
  font-size: 30px;
  font-family: monospace;
  color: chartreuse;
  margin-bottom: 10px;
}
p {
  font-size: 16px;
  font-family: monospace;
  color: #000;
  margin-bottom: 20px;
}
</style>