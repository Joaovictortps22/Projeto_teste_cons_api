<template>
  <v-app>
    <v-app-bar
      app
      color="blue"
      dark
    >
      <div class="d-flex align-center" id="Titulo">
          PROJETO TESTE
      </div>

      <v-spacer></v-spacer>

      
        
    </v-app-bar>

    <v-content>
      <head_page/>
    </v-content>
  </v-app>
</template>

<script>
import head_page from './components/head_page';

export default {
  name: 'App',

  components: {
    head_page,
  },

  data: () => ({
    //
  }),
};
</script>

<style>
    #Titulo{
      font-size: 22px;
    }
</style>
