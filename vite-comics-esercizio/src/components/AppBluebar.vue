<script>
export default {
  data(){
    
  }
}
</script>


<template>
  <section>
    <div class="container container-blue">
      <div class="bluebar">
        <ul class="row row-bluebar">
          <li class="bluebar-item">
            <img src="/images/buy-comics-digital-comics.png" alt="">
            <span>
              digital comics
            </span>
          </li>
          <li class="bluebar-item">
            <img src="/images/buy-comics-merchandise.png" alt="">
            <span>
              dc merchandise
            </span>
          </li>
          <li class="bluebar-item">
            <img src="/images/buy-comics-subscriptions.png" alt="">
            <span>
              subscription
            </span>
          </li>
          <li class="bluebar-item">
            <img id="position-logo" src="/images/buy-comics-shop-locator.png" alt="">
            <span>
              comic shop locator
            </span>
          </li>
          <li class="bluebar-item">
            <img src="/images/buy-dc-power-visa.svg" alt="">
            <span>
              dc power visa
            </span>
          </li>
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