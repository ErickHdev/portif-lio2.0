<script setup>
import { RouterView } from 'vue-router'

</script>

<template>
  <!--navbar smartphone -->
  <NavBar />
  <MyApresentation />
  <AboutMe />
  <Skills />


  <RouterView />
</template>

<script>
import NavBar from './components/NavBar.vue'
import MyApresentation from './components/MyApresentation.vue'
import AboutMe from './components/AboutMe.vue'
import Skills from './components/Skills.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    MyApresentation,
    AboutMe,
    Skills
  }
}
</script>

<style scoped>

</style>
