<script setup>
import { RouterView } from 'vue-router'

</script>

<template>
  <!--navbar smartphone -->
  <NavBar />
  <MyApresentation />

  <RouterView />
</template>

<script>
import NavBar from './components/NavBar.vue'
import MyApresentation from './components/MyApresentation.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    MyApresentation
  }
}
</script>

<style scoped>

</style>
