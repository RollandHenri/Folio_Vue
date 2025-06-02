<script setup>
import Link from "../components/Link.vue";
</script>

<template>
  <nav>
    <Logo />
    <Link class="navbar-link" />
    <div class="navbar-after">
      <img src="../../public/img/logo.webp" alt="Logo Rolland-Dev" />
    </div>
  </nav>
</template>

<style scoped>
nav {
  position: relative;
}

.navbar-after {
  position: absolute;
  bottom: -40%;
  left: 50%;
  transform: translate(-50%, 50%);
  width: 0;
  height: 0px;
  opacity: 0;
  background-color: rgb(214, 114, 211);
  border-bottom-right-radius: 250px;
  border-bottom-left-radius: 250px;
  animation: reveal 0.8s ease forwards;
  animation-delay: 0.8s;
}

.navbar-after img {
  position: fixed;
  left: 50%;
  bottom: 0;
  transform: translateX(-50%);
  padding-top: 10px;
  margin: 0 auto;
  width: 100px;
  opacity: 0;
  animation: fadeIn 0.8s ease forwards 1.4s;
}

.navbar-link {
  left: 0;
  top: 0;
  width: 100%;
  height: 70px;
  background-color: rgb(214, 114, 211);
  transition: all 0.6s ease 1s;
}

@keyframes reveal {
  0% {
    width: 0;
    height: 0;
    opacity: 0;
  }
  100% {
    width: 180px;
    height: 80px;
    opacity: 1;
  }
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}
</style>
