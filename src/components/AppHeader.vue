<script>
  export default {
    data(){
      return{
        
        menuItems: [

          {
            itemClass: 'menu-item',
            itemSpec: 'character',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'comics',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'movies',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'tv',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'games',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'collectibles',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'videos',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'fans',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'news',
          },
          {
            itemClass: 'menu-item',
            itemSpec: 'shop',
          },

        ]


      }
    }
  }
</script>


<template>
  <header>
    <section>
      <div class="container">

        <div class="row row-header">

          <img src="/images/dc-logo.png" alt="">

          <ul class="menu">
            <li v-for="(el,i) in menuItems" class="menu-item">{{ menuItems[i].itemSpec }}</li>
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
    text-decoration: underline;
  }

  .active{
    color: #0282F9;
  }

</style>