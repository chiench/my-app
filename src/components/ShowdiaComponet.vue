<template>
  <div class="text-center">
      <v-btn
          color="red lighten-2"
          dark
        
          @click="dialog = true"
        >
          Click Me
        </v-btn>
    <v-dialog
    style="text-align: center"
    transition="dialog-top-transition"
      v-model="dialog"
      width="500"
    >
  
  
      


      <v-card>
        <v-card-title class="text-h5 grey lighten-2">
          Privacy Policy
        </v-card-title>
<v-row>
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
      

    

        <v-divider></v-divider>

        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn
            color="primary"
            text
            @click="dialog = false"
          >
            I accept
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>
  </div>
  
</template>
<script>
export default {
  data() {
    return {
      dialog: false,
    };
  },
};
</script>

<style>
</style>