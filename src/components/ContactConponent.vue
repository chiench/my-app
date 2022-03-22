<template>
  <v-container class="mt-5">
    <v-row>
      <v-col style="text-align: center" lg="12">
        <div>
          <h2>Contact Us</h2>
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ea, quam!
          </p>
        </div>
      </v-col>
      <v-col lg="6">
        <img src="https://picsum.photos/510/300?random" alt="" />
      </v-col>
      <v-col lg="6">
    
  <v-form
    ref="form"
    
    lazy-validation
  >
    <v-text-field
     
      label="Name"
      required
    ></v-text-field>

    <v-text-field
     
      label="E-mail"
      required
    ></v-text-field>

    <v-select
      
      
      
      label="Item"
      required
    ></v-select>


    <v-btn
   
      color="success"
      class="mt-4"
    
    >
      Validate
    </v-btn>


    </v-form>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {};
</script>

<style>
</style>