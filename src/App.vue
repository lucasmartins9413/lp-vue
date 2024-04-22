<template>
  <div id="app">
    <Header title="Dog Dev"></Header>
    
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

</style>