<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import NavbarVue from './components/Navbar.vue';
import ContentVue from './components/Content.vue';
import FooterVue from './components/Footer.vue'
</script>

<template>
  <div class="flex flex-col">
    <NavbarVue />
    <ContentVue />
    <div class="divider"></div>
    <FooterVue />
  </div>
</template>

<style scoped></style>
