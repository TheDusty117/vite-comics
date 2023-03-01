<script setup>
// import HelloWorld from './components/HelloWorld.vue'
//1. importo il componente
import AppHeader from './components/AppHeader.vue'

export default {

  components: {
    // 2. registro il componente importato prima
    AppHeader

  },
  
}

</script>

<template>

  <!--3. utilizzo il componente -->
  <AppHeader/>

</template>

<style scoped>

</style>
