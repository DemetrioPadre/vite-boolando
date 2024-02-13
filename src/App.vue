<script>
import { store } from './store';
import axios from 'axios';
// inseriamo tutte le sezione di IMPORT
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppCard from './components/AppCard.vue';



export default {
  data() {
    return {
      products: []
    };
  },

  components: { AppHeader, AppMain, AppCard, AppFooter },

};
</script>



<template>
  <AppHeader></AppHeader>
  <div v-for="product in products"> {{ product.name }}</div>
  <AppMain></AppMain>


  <AppFooter></AppFooter>
</template>



<style lang ="scss">
@use'./styles/general.scss';
</style>

