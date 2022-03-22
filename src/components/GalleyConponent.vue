<template>
  <v-container class="mt-5">
    <v-row justify="center">
      <v-col style="text-align: center" lg="12">
        <div style="text-align: center">
          <h2>About Us</h2>
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ea, quam!
          </p>
        </div>
      </v-col>

        <v-col v-for="n in 9" :key="n" class="d-flex child-flex text-center" cols="2">
          <v-img
            :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
            :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
            aspect-ratio="1"
            class="grey lighten-2"
          >
            <template v-slot:placeholder>
              <v-row class="fill-height ma-0" align="center" justify="center">
                <v-progress-circular
                  indeterminate
                  color="grey lighten-5"
                ></v-progress-circular>
              </v-row>
            </template>
          </v-img>
        </v-col>
      </v-row
  ></v-container>
</template>

<script>
export default {};
</script>

<style>
</style>