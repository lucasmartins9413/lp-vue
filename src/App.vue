<template>
  <div id="app">
    <Header title="Meu Site"></Header>
    
    <RouterView />

    <Footer></Footer>
  </div>
</template>

<script setup>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import { RouterView } from 'vue-router'
</script>

<style>
/* Estilos globais */
</style>