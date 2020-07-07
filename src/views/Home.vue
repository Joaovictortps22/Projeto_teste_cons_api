<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import head_page from '@/components/head_page.vue'
import Vuetify from 'vuetify'

export default {
  name: 'Home',
  components: {
    head_page
  }
}
</script>
