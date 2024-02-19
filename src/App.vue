<script setup>
import { RouterView } from 'vue-router'

</script>

<template>
  <!--navbar smartphone -->
  <NavBar />
  <MyApresentation />
  <AboutMe />
  <Skills />
  <Projetos />

  <RouterView />
</template>

<script>
import NavBar from './components/NavBar.vue'
import MyApresentation from './components/MyApresentation.vue'
import AboutMe from './components/AboutMe.vue'
import Skills from './components/Skills.vue'
import Projetos from './components/Projetos.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    MyApresentation,
    AboutMe,
    Skills,
    Projetos
  }
}
</script>

<style scoped>

</style>
