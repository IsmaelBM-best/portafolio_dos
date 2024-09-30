<script>
import Footer from './components/Footer.vue';
import Header from './components/Header.vue';

export default {
  components: {
    Header,
    Footer
  },
  data(){
    return {

    }
  }
}
</script>

<template>
  <div class="principal_container">
    <Header />
    <div class="introduce_myself">
      <h1>Hola, soy Ismael Blandon Moreno:</h1>
      <p>Soy desarrollador de software especializado en el front-end, con experiencia en la creación de interfaces de usuario intuitivas y eficientes.</p>
    </div>
    <div class="certified_container">
      <img class="one" src="/src/assets/full-stack.jpeg" alt="">
      <img class="two" src="/src/assets/react.jpeg" alt="">
      <img class="three" src="/src/assets/fundamentos.jpeg" alt="">
    </div>
    <Footer />
  </div>
</template>

<style>
@import '/src/styles/main.css';
</style>
