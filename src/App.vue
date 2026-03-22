<script setup lang="ts">
import { Navbar, Footer } from './components'
</script>

<template>
  <Navbar />
  <div class="content">
    <router-view />
  </div>
  <Footer />
</template>

<style scoped lang="scss">
.content {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  height: 100%;
  overflow-y: auto;
  overflow-x: hidden;
}
</style>
