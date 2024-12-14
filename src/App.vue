<template>
  <v-app class="bg-white">
    <Header />
    <v-main>
      <router-view />
    </v-main>
    <Footer />
  </v-app>
</template>

<script setup>
  import Header from './components/Header.vue'
  import Footer from './components/Footer.vue'
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  margin: 0;
  padding: 0;
  width: 100%;
  overflow-x: hidden;
}
</style>