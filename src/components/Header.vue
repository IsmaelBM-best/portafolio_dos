<script>
export default {
  data(){
    return {
      modal_contact: false
    }
  },
  methods: {
    modalToggle(){
      this.modal_contact = !this.modal_contact
    }
  }
}
</script>

<template>
  <div class="header_ibm">
    <img src="/src/assets/logo_isma.svg" alt="">
    <button class="contact_button" @click="modalToggle">
      <img src="/src/assets/options.png" alt="">
    </button>
  </div>
  <div class="contact_modal" v-if="modal_contact">
    <div class="close_container">
      <button class="close" @click="modalToggle">
        <img src="/src/assets/close.png" alt="">
      </button>
    </div>
    <div class="img_container">
      <img src="/src/assets/yo_transparent.png" alt="">
    </div>
    <div class="social_media">
      <h2>!Échale un vistazo a mis redes sociales y proyectos!</h2>
      <div class="links_container">
        <a href="https://www.linkedin.com/in/ismael-blandon-moreno-944605266/" target="_blank">
          <img src="/src/assets/linkedin.png" alt="">
        </a>
        <a href="https://github.com/IsmaelBM-best?tab=repositories" target="_blank">
          <img src="/src/assets/github.png" alt="">
        </a>
        <a href="https://app.netlify.com/teams/ismaelbm432/sites" target="_blank">
          <img src="/src/assets/netlify-icon.png" alt="">
        </a>
      </div>
    </div>
    <div class="cv">
      <p>Disponible para conversar sobre cómo puedo aportar a tu equipo. Escríbeme directamente a mi WhatsApp.</p>
      <a href="https://wa.me/3007982609?text=Hola%20me%20gustaría%20hablar%20sobre%20tu%20portafolio" target="_blank">
        Enviar mensaje
        <img src="/src/assets/whatsapp.png" alt="">
      </a>
    </div>
  </div>
</template>

<style>
@import '/src/styles/header.css';
</style>
