<template>
  <v-container class="mt-5">
    <v-row>
      <v-col lg="12">
        <div style="text-align: center">
          <h2>About Us</h2>
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ea, quam!
          </p>
        </div>
      </v-col>
      <v-col lg="4" v-for="i in 3" :key="i">
        <v-card :loading="loading" class="mx-auto my-12" max-width="374">
          <template slot="progress">
            <v-progress-linear
              color="deep-purple"
              height="10"
              indeterminate
            ></v-progress-linear>
          </template>

          <v-img
            height="150"
            src="https://cdn.vuetifyjs.com/images/cards/cooking.png"
          ></v-img>
          <v-card-text>
            <v-card-title>Product</v-card-title>

            <div class="my-4 text-subtitle-1">$ • Italian, Cafe</div>

            <div>
              Small plates, salads & sandwiches - an intimate setting with 12
              indoor seats plus patio seating.
            </div>
          </v-card-text>
          <v-card-text>
            <v-row align="center" class="mx-0"> </v-row>
          </v-card-text>

          <v-divider class="mx-4"></v-divider>

          <v-card-actions>
            <v-btn color="success" rounded> Add </v-btn>
            <v-spacer />
            <v-rating
              :value="4.5"
              color="amber"
              dense
              half-increments
              readonly
              size="14"
            ></v-rating>
          </v-card-actions>
        </v-card>
      </v-col>     
    </v-row>
  </v-container>
</template>

<script>
export default {};
</script>

<style>
</style>