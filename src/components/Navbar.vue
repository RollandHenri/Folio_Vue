<script setup>
import Link from "../components/Link.vue";
</script>

<template>
  <nav>
    <Link class="navbar-link" />
  </nav>
</template>

<style scoped>
.navbar-link {
  left: 0;
  top: 0;
  width: 100%;
  height: 60px;
  background-color: #7e1e5196;
  border-top-left-radius: 25%;
  border-top-right-radius: 25%;
}
</style>
