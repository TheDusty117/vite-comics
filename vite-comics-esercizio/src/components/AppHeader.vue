<script>
  export default {

  }
</script>


<template>
  <header>
    <section>
      <div class="container">

        <div class="row row-header">

          <img src="/images/dc-logo.png" alt="">

          <ul class="menu">
            <li class="menu-item">character</li>
            <li class="menu-item active">comics</li>
            <li class="menu-item">movies</li>
            <li class="menu-item">tv</li>
            <li class="menu-item">games</li>
            <li class="menu-item">collectibles</li>
            <li class="menu-item">videos</li>
            <li class="menu-item">fans</li>
            <li class="menu-item">news</li>
            <li class="menu-item">shop</li>
          </ul>

        </div>
      </div>
    </section>
  </header>
</template>


<style lang="scss" scoped>

  section{
    background-color: white;
    color: black;
    padding: 15px 0px;
  }

  .row-header{
    justify-content: space-between;
  }

  .menu{
    display: flex;
    align-items: center;
    gap: 20px;
  }
  .menu-item{
    font-size: 16px;
    text-transform: uppercase;
    font-weight: 700;
  }

  .menu-item:hover{
    color: #0282F9;
  }

  .active{
    color: #0282F9;
  }

</style>