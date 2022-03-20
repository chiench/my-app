<template>
  <v-app>
<HeaderComponent/>
    <v-main>
      <InfoComponent/>
      <AboutComponent/>
      <PortfolioComponent/>
    </v-main>
  </v-app>
</template>
<script>
import HeaderComponent from './components/HeaderComponent.vue'
import InfoComponent from './components/InfoComponent.vue'
import AboutComponent from './components/AboutComponent.vue'
import PortfolioComponent from './components/PortfolioComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    InfoComponent,
    AboutComponent,
    PortfolioComponent,
   
  },

  data: () => ({
    //
  }),
};
</script>
