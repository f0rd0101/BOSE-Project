<script setup lang="ts">
import { defineProps,computed } from 'vue';

const props = defineProps({
    isOpen: Boolean,
})
const emit = defineEmits(['close'])
const modalClass = computed(()=>{
    return props.isOpen ?  'is-open' : ''
})
</script>


<template>
         <div class="menu" id="menu"  :class="modalClass">
      <div class="div-img-2">
        <img src="../../assets/images/bose-logo.png" alt="bose-logo" class="img-logo" />
        <button type="button" class="burger-menu-button" @click="$emit('close')">
          <a href="#home">
            <svg class="burger-menu icon-close">
              <use href="../../assets/images/svgpic.svg#icon-Icon-Close"></use>
            </svg>
          </a>
        </button>
      </div>
      <div>
      <ul class="menu-ul">
        <li class="menu-link">
          <a href="#home" class="link-nav">Home</a>
        </li>
        <li class="menu-link">
          <a href="#recommended" class="link-nav">recommended</a>
        </li>
        <li class="menu-link">
          <a href="#products" class="link-nav">Categories</a>
        </li>
        <li class="menu-link">
          <a href="#benefits" class="link-nav">How to buy</a>
        </li>
      </ul>
      </div>
    </div>
</template>


<style scoped>

.div-img-2 {
  display: flex;
  justify-content: space-between;
}
.burger-menu-button {
  background: transparent;
  border: none;
}
.img-logo {
  width: 127px;
  height: 16px;
}
.menu-ul {
  display: flex;
  flex-direction: column;
  gap: 25px;
  margin: 0;
  padding-bottom: 90px;

  list-style-type: none;
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
  text-decoration: none;
}
.burger-menu {
  width: 24px;
  height: 24px;
}

@media screen and (min-width: 472px) {
  /* =================Header menu settings================== */
  .burger-menu {
    fill: black;
  }
  .menu-ul {
    gap: 20px;
  }
}
@media screen and (min-width: 1200px) {
  img {
    width: 100%;
  }
}
@media screen and (min-width: 1260px) {
  /* =================Header================== */
  .burger-menu {
    width: 24px;
    height: 24px;
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
    padding-left: 104px;
  }
  .is-open {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    /* padding: 64px 120px; */
    padding: 32px 16px;
    background-color: #e8eff9;
    position: fixed;
    top: 0;
    right: 0;
    left: 0;
    transform: translateX(-100%);
    transition: transform 500ms;
    height: 100vh;
    box-sizing: border-box;
  }
  .is-open:target {
    transform: translateX(0);
  }
}
</style>