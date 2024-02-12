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

    };
  },

  components: { AppHeader, AppMain, AppCard, AppFooter },
  created() {
    axios.get('http://localhost:3000/products');
  }
};



</script>



<template>
  <AppHeader></AppHeader>

  <AppMain></AppMain>


  <AppFooter></AppFooter>
</template>



<style lang ="scss">
@use'./styles/general.scss';
</style>

