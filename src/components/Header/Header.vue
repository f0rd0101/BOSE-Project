<script setup lang="ts">
import HeaderModal from '../HeaderModal/HeaderModal.vue'
import { ref } from 'vue';

const modalOpen = ref(false)

const modalSwitchToogle = ()=>{
  modalOpen.value = !modalOpen.value
}

</script>


<template>
    <header class="header-section container" id="home">
      <div class="div-img">
        <img src="../../assets/images/bose-logo.png" alt="bose-logo" class="bose-logo" />
        <button type="button" class="burger-menu-button" @click="modalSwitchToogle">
          <a href="#menu">
            &equiv;
          </a>
        </button>
      </div>
      <div>
        <svg class="sound-svg">
          <use href="../../assets/images/svgpic.svg#icon-Sound-waves"></use>
        </svg>
        <h1 class="slogan">
          The world shades.
          <br />
          Your music shines.
        </h1>
      </div>
    <HeaderModal v-if="modalOpen" :isOpen="modalOpen" @close ="modalOpen = false"/>
    </header>
</template>



<style scoped>
.burger-icon-320 {
  fill: white;
}

.header-section {
  width: 100%;
  height: 500px;
  padding: 32px 16px;
  box-sizing: border-box;
  background-image: url("../../assets/images/background-header.png");
  background-repeat: no-repeat;
  background-position: 40%;
  background-size: cover;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  min-width: 320px;
}
.burger-menu {
  width: 24px;
  height: 24px;
}
.burger-menu-button {
  font-size: 24px;
  line-height: 1;
  background: none;
  border: none;
  cursor: pointer;
}
.sound-svg {
  width: 32px;
  height: 38px;
}
.slogan {
  color: #292929;

  font-family: Inter;
  font-size: 32px;
  font-style: italic;
  font-weight: 800;
  line-height: 100%; /* 32px */
  letter-spacing: -0.03125em;
}
.bose-logo {
  width: 127px;
  height: 16px;
}
.div-img {
  display: flex;
  justify-content: space-between;
}
  img {
    width: 100%;
  }
  a {
    text-decoration: none;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }

  .div-img-2 {
    display: flex;
    justify-content: space-between;
    margin-bottom: 64px;
  }
  .link-nav {
    color: #292929;

    font-family: Inter;
    font-size: 22px;
    font-style: normal;
    font-weight: 700;
    line-height: 1em;
    letter-spacing: 0.09em;
    text-transform: uppercase;
  }
  .menu-ul {
    display: flex;
    flex-direction: column;
    gap: 32px;
    margin: 0;
  }

</style>