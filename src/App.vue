<script setup>
import { RouterView } from 'vue-router'

</script>

<template>
  <!--navbar smartphone -->
  <NavBar />
  <MyApresentation />
  <AboutMe />
  <Skills />

  <Projetos class= "Pdt"/>
  <ProjetosMobile class="Pmo" />
  <Contact />
  <RouterView />
</template>

<script>
import NavBar from './components/NavBar.vue'
import MyApresentation from './components/MyApresentation.vue'
import AboutMe from './components/AboutMe.vue'
import Skills from './components/Skills.vue'
import Projetos from './components/Projetos.vue'
import Contact from './components/Contact.vue'
import ProjetosMobile from './components/ProjetosMobile.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    MyApresentation,
    AboutMe,
    Skills,
    Projetos,
    ProjetosMobile,
    Contact
  }
}
</script>

<style scoped>

@media (hover: hover) {

}

@media (max-width: 1024px) {

}

@media (max-width: 800px) {

}
/* media query smartphone */

@media (max-width: 600px) {

}

@media (max-width: 600px) {

}
</style>
