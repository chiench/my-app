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
      <v-col lg="12" style="text-align: center" >
        <img src="https://picsum.photos/510/300?random" alt="" />
      </v-col>
      <v-col lg="12">
    <ShowdiaComponet/>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import ShowdiaComponet from './ShowdiaComponet.vue'

export default {
  
   data: () => ({
    //
  }),
  components:{
ShowdiaComponet
  },
 
  methods: {
    opendialog(){
      console.log(2)
    }
  },
};
</script>

<style>
</style>