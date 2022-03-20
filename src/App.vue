<template>
  <v-app>
<HeaderComponet/>
    <v-main>
      <InfoComponet/>
    </v-main>
  </v-app>
</template>
<script>
import HeaderComponet from './components/HeaderComponet.vue'
import InfoComponet from './components/InfoComponet.vue'

export default {
  name: 'App',
  components: {
    HeaderComponet,
    InfoComponet,
   
  },

  data: () => ({
    //
  }),
};
</script>
