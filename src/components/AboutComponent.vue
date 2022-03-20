<template>
  <v-container class="mt-3 ">
      <v-row>
          <v-col lg="6">
            <img src="../assets/logo.png" width="100%" alt="" />
          </v-col>
          <v-col class="pl-10" lg="6">
              <v-subheader class="sub"> About Us </v-subheader>
              <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ea, quam!</p>
              <v-list>
                  <v-list-item v-for="i in 3" :key="i" >
                      <v-icon class="mr-3" color="success">mdi-check-all</v-icon>
                      <v-list-item-title>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Sequi, tenetur.</v-list-item-title>
                  </v-list-item>
              </v-list>
          </v-col>
      </v-row>
  </v-container>
</template>

<script>
export default {

}
</script>

<style scoped>
.sub{
    font-family: monospace;
    font-size: 40px;
    font-weight: bold;
    color:#000;
    margin : 27px 0px;
}

</style>