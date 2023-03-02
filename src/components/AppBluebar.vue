<script>


import BluebarCard from './BluebarCard.vue';

export default {


  components: {
    BluebarCard,
  },


  data(){
    return{

      barObjects: [
        {
          img: '/images/buy-comics-digital-comics.png',
          description: 'digital comics'
        },
        {
          img: '/images/buy-comics-merchandise.png',
          description: 'dc merchandise'
        },
        {
          img: '/images/buy-comics-subscriptions.png',
          description: 'subscription'
        },
        {
          img: '/images/buy-comics-shop-locator.png',
          description: 'comic shop locator'
        },
        {
          img: '/images/buy-dc-power-visa.svg',
          description: 'dc power visa'
        },
      ]

    }
  }
}
</script>


<template>
  <section>
    <div class="container container-blue">
      <div class="bluebar">
        <ul class="row row-bluebar">
          
          <!-- <li v-for="(barObject,i) in barObjects" :key="i" class="bluebar-item">
            <img class="bluebar-logo" :src="barObject.img" alt="">
            <span>
              {{ barObject.description }}
            </span>
          </li> -->

          <BluebarCard v-for="(obj,i) in barObjects" :key="i" :img="obj.img" :description="obj.description"   />
          
        </ul>
      </div>
    </div>

  </section>
</template>


<style lang="scss" scoped>


ul{

} 
  li{
    display: flex;
    align-items: center;
    gap: 10px;
  }

  #position-logo{
    width: 35px;
  }
  

  span{
    font-size: 15px;
    text-transform: uppercase;
    font-weight: 600;
  }

section{
  background-color:  #0282F9;
}

  .bluebar{
    min-height: 100px;
    width: 100%;
  }

  img{
    width: 50px;
  }


.row-bluebar{
  justify-content: space-evenly;
  align-items: center;
  height: 170px;
  gap: 20px;
}  





</style>