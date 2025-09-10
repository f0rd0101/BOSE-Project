<script>
</script>
<template>
    <header class="header-section container" id="home">
      <div class="div-img">
        <img src="../../assets/images/bose-logo.png" alt="bose-logo" class="bose-logo" />
        <button type="button" class="burger-menu-button">
          <a href="#menu">
            <svg class="burger-menu burger-icon-320">
              <use href="../../assets/images/svgpic.svg#icon-Icon-Burger-menu"></use>
            </svg>
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
        <div class="menu is-open" id="menu">
      <div class="div-img-2">
        <img src="../../assets/images/bose-logo.png" alt="bose-logo" class="img-logo" />
        <button type="button" class="burger-menu-button">
          <a href="#home">
            <svg class="burger-menu icon-close">
              <use href="../../assets/images/svgpic.svg#icon-Icon-Close"></use>
            </svg>
          </a>
        </button>
      </div>

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
    </header>
</template>

<style scoped>
.is-open {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding: 35px 18px;
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
.div-img-2 {
  display: flex;
  justify-content: space-between;
}
.img-logo {
  width: 127px;
  height: 16px;
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
.menu-ul {
  display: flex;
  flex-direction: column;
  gap: 25px;
  margin: 0;
  padding-bottom: 90px;

  list-style-type: none;
}
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
  background: transparent;
  border: none;
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
@media screen and (min-width: 472px) {
  /* =================Header menu settings================== */
  .burger-menu {
    fill: black;
  }
  .menu-ul {
    gap: 20px;
  }
  .rec-section {
    padding: 0 20px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .product-li {
    display: flex;
    justify-content: center;
    flex-direction: column;
    width: 400px;
  }
  .product-ul :nth-child(-n + 3) {
    display: flex;
    align-items: center;
  }
}
@media screen and (min-width: 1200px) {
  .product-ul {
    flex-direction: row;
  }
  .product-li {
    width: 300px;
  }
  img {
    width: 100%;
  }
}
@media screen and (min-width: 1260px) {
  /* =================Header================== */
  .slogan {
    color: #292929;

    font-family: Inter;
    font-size: 48px;
    font-style: italic;
    font-weight: 800;
    line-height: 100%; /* 48px */
    letter-spacing: -0.03125em;
  }
  .burger-menu {
    width: 24px;
    height: 24px;
  }
  .burger-menu-button {
    background: transparent;
    border: none;
  }
  .div-img {
    display: flex;
    justify-content: space-between;
  }

  .sound-svg {
    width: 64px;
    height: 76px;
  }
  a {
    text-decoration: none;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  .is-open {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 64px 120px;
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
}
</style>