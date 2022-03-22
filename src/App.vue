<template>
  <v-app>
<HeaderComponent/>
    <v-main>
      <InfoComponent/>
      <AboutComponent/>
      <PortfolioComponent/>
      <ShopComponent/>
      <GalleyConponent/>
      <ContactConponent/>
    </v-main>
    <v-divider class="mt-20" />
      <FooterConponent/>
    
  </v-app>
</template>
<script>
import HeaderComponent from './components/HeaderComponent.vue'
import InfoComponent from './components/InfoComponent.vue'
import AboutComponent from './components/AboutComponent.vue'
import PortfolioComponent from './components/PortfolioComponent.vue'
import ShopComponent from './components/ShopComponent.vue'
import GalleyConponent from './components/GalleyConponent.vue'
import ContactConponent from './components/ContactConponent.vue'
import FooterConponent from './components/FooterConponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    InfoComponent,
    AboutComponent,
    PortfolioComponent,
    ShopComponent,
    GalleyConponent,
    ContactConponent,
    FooterConponent,
   
  },

  data: () => ({
    //
  }),
};
</script>
