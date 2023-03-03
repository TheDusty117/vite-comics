<script>
  export default{
    
    props: {
      
      title:String,
      links:Array,
      
    }

  }
</script>

<!-- 1. copio il mio html togliendo v-for (che poi usero' in seguito alla creazione di questo prop)-->
<template>


<ul class="infos-list">

<h2>{{ title }}</h2>
<li v-for="link in links" key="i" class="infos-item">
  <a href="">{{ link }}</a>
</li>

</ul>


</template>



<!--2. copio lo style dell'elemento da "proppare"-->
<style lang="scss" scoped>

.infos-item{
    font-size: 15px;
    color: gray;
  }

  h2{
    text-transform: uppercase;
    font-size: 20px;
  }


</style>