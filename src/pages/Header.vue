<script setup>
import Navbar from "../components/Navbar.vue";
</script>

<template>
  <div class="header-hero">
    <div class="header-hero-logo">
      <img src="../../public/img/logo.webp" alt="Logo Rolland Dev" />
    </div>
    <div class="header-hero-title-top"></div>
    <div class="header-hero-profil">
      <img
        src="../../public/img/profil-pic.webp"
        alt="photo de profile de rolland dev"
      />
    </div>
    <div class="header-hero-title-bottom">
      <p>Bonjour, je suis</p>
      <h1>Henri Rolland</h1>
      <p>Développeur Web Front End <span>React & Vue.JS</span></p>
    </div>
    <Navbar class="header-hero-navbar" />
  </div>
</template>

<style scoped>
.header-hero {
  position: relative;
  height: 100vh;
  background: white;
}

.header-hero-logo {
  width: 100%;
  height: 20%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0 auto;
}

.header-hero-logo img {
  width: 40%;
}

.header-hero-profil {
  position: absolute;
  left: 50%;
  top: 45%;
  width: 80%;
  transform: translate(-50%, -50%);
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0 auto;
  z-index: 5;
}

.header-hero-profil img {
  width: 90%;
  height: auto;
  margin: 0 auto;
  border-radius: 100%;
}
.header-hero-bottom {
  height: 60%;
}

.header-hero:after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 80%;
  clip-path: polygon(100% 49%, 100% 100%, 0 100%, 0 20%);
  background: linear-gradient(
    171deg,
    rgb(255, 255, 255) 0%,
    rgb(87, 22, 55) 37%,
    rgb(0, 0, 0) 70%
  );
}

.header-hero-title-bottom {
  position: absolute;
  left: 50%;
  bottom: 15%;
  transform: translate(-50%, -50%);
  width: 90%;
  text-align: center;
  z-index: 5;
}

.header-hero-navbar {
  position: fixed;
  bottom: 0;
  width: 100%;
  z-index: 1;
}
</style>
