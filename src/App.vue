<script setup>
import { RouterView } from 'vue-router'

</script>

<template>
  <!--navbar smartphone -->
  <NavBar />
  <Apresentation />

  <RouterView />
</template>

<script>
import NavBar from './components/NavBar.vue'
import Apresentation from './components/Apresentation.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    Apresentation
  }
}
</script>

<style scoped>
NavBar{
  position: fixed;
}
</style>
