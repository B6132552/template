<template>
  <div>
    <div class="hero-bg">
      <Header />
      <TheHero />
    </div>
    <SectionFirst/>
    <Footer />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue"
import Header from './components/Header.vue'
import TheHero from './components/TheHero.vue'
import Footer from "./components/Footer.vue"
import SectionFirst from "./components/SectionFirst.vue"
export default defineComponent({
  components: { Header, TheHero, Footer,SectionFirst }
})
</script>

<style>
nav {
  padding: 0px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

.hero-bg {
  background-image: url("../src/assets/image/bg.png");
  background-size: cover;
  width: 100%;
  height: 100vh;
}
</style>
