<script>
import { store } from './store';
import axios from 'axios';
// inseriamo tutte le sezione di IMPORT
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue';
import AppCard from './components/AppCard.vue';
import AppModal from './components/AppModal.vue';



export default {
  data() {
    return {
      products: [],
      store,
    };
  },

  components: { AppHeader, AppMain, AppCard, AppFooter, AppModal },

};
</script>



<template>
  <AppHeader></AppHeader>
  <div v-for="product in products"> {{ product.name }}</div>
  <AppModal v-if="store.modal.show"></AppModal>
  <AppMain></AppMain>


  <AppFooter></AppFooter>
</template>



<style lang ="scss">
@use'./styles/general.scss';
</style>

