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

        <div class="text-center">
    <v-menu disabled top offset-y>
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="primary"
          dark
          v-bind="attrs"
          v-on="on"
        >
          API Correios
        </v-btn>
      </template>

      <v-list>
        <v-list-item
          v-for="(item, index) in items"
          :key="index"
          @click=""
        >
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-menu>
  </div>

    <div class="text-center">
    <v-menu disabled top offset-y>
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="primary"
          dark
          v-bind="attrs"
          v-on="on"
        >
          Dropdown
        </v-btn>
      </template>

      <v-list>
        <v-list-item
          v-for="(item, index) in items"
          :key="index"
          @click=""
        >
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-menu>
  </div>

    <div class="text-center">
    <v-menu disabled top offset-y>
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="primary"
          dark
          v-bind="attrs"
          v-on="on"
        >
          Dropdown
        </v-btn>
      </template>

      <v-list>
        <v-list-item
          v-for="(item, index) in items"
          :key="index"
          @click=""
        >
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-menu>
  </div>
        
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
    .text-center{
      margin-right: 10px;
    }
</style>
