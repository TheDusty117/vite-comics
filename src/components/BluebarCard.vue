<script>
  export default{
    
    props: {
      img: String,
      description: String,
    }

  }
</script>

<!-- 1. copio il mio html togliendo v-for (che poi usero' in seguito alla creazione di questo prop)-->
<template>
  <li class="bluebar-item">
    <img class="bluebar-logo" :src="img" alt="">
    <span>
      {{ description }}
    </span>
  </li>
</template>



<!--2. copio lo style dell'elemento da "proppare"-->
<style lang="scss" scoped>

li{
    display: flex;
    align-items: center;
    gap: 10px;
  }


  span{
    font-size: 15px;
    text-transform: uppercase;
    font-weight: 600;
  }


  .bluebar{
    min-height: 100px;
    width: 100%;
  }

  img{
    width: 50px;
  }


</style>