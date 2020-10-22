<template>
  <v-app>
    <Navegacion/>
    <router-view> </router-view>
  </v-app>
</template>

<script>
import Navegacion from './components/Navegacion.vue';

export default {
  name: 'App',

  components: {
    Navegacion,
  },

  data: () => ({
    //
  }),
};
</script>
