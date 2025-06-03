<script setup>
import Navbar from "../pages/Navbar.vue";
</script>

<template>
  <div class="header-hero">
    <div class="header-hero-logo">
      <img src="../../public/img/logo.webp" alt="Logo Rolland Dev" />
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
  width: 50%;
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

.header-hero-navbar {
  position: fixed;
  bottom: 0;
  width: 100%;
  z-index: 1;
}
</style>
