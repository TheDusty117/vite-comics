<script>
// import HelloWorld from './components/HelloWorld.vue'
//1. importo il componente
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppBluebar from './components/AppBluebar.vue'
import AppFooter from './components/AppFooter.vue'


export default {

  components: {
    // 2. registro il componente importato prima
    AppHeader,
    AppMain,
    AppBluebar,
    AppFooter

  },
  
}

</script>

<template>

  <!--3. utilizzo il componente -->
  <AppHeader/>

  <AppMain/>

  <AppBluebar/>

  <AppFooter/>


</template>

<style lang="scss">
/* stili comuni su tutto il sito web */

//includo il file general
@use './style/general.scss';

</style>
