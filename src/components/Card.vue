<script>
  export default{
    
    props: {
      series: String,
      thumb: String,
    }

  }
</script>

<!-- 1. copio il mio html togliendo v-for (che poi usero' in seguito alla creazione di questo prop)-->
<template>
  <li class="card">
    <div class="comic-image">
      <img class="comic-image" :src="thumb" alt="">
    </div>
    <h3 class="card-title">{{ series }}</h3>
  </li>
</template>



<!--2. copio lo style dell'elemento da "proppare"-->
<style lang="scss" scoped>

.card{
    padding: 15px;
  }

  .comic-image{
    object-fit: cover;
    width: 200px;
    height: 200px;
  }

  .card-title{
    font-size: 18px;
    text-transform: uppercase;
  }

</style>