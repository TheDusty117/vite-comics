<script>

// 1... importare il componente Card
import Card from './Card.vue'

export default {

  // 2.. registrare componente
  components: {
    Card
  },

  data() {
    return {
      comics: [
        {
          thumb: "/images/action-comics.jpeg",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book"
        },
        {
          thumb: "/images/vampire-1976.jpg",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book"
        },
        {
          thumb: "/images/acquaman.jpg",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel"
        },
        {
          thumb: "/images/batgirl.jpg",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book"
        },
        {
          thumb: "/images/batman.jpg",
          price: "$3.99",
          series: "Batman",
          type: "comic book"
        },
        {
          thumb: "/images/batman-beyond.jpg",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book"
        },
        {
          thumb: "/images/batman-superman.jpg",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book"
        },
        {
          thumb: "/images/batman-superman-annual.jpg",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book"
        },
        {
          thumb: "/images/batman-joker-warzone.jpg",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book"
        },
        {
          thumb: "/images/batman-three-jokers.jpg",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book"
        },
        {
          thumb: "/images/harley-quinn.jpg",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book"
        },
        {
          thumb: "/images/catwoman.jpg",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel"
        }
      ]
    }
  }
}
</script>


<template>
  <main>

    <!--HERO SECTION-->
    <section>
      <div  class="hero-immagine" ></div>
    </section>

    <!--CONTENT SECTION-->
    <section class="grid-sect">
      <div class="container container-griglia">
      <div class="current-series">
        <h3>
          CURRENT SERIES
        </h3> 
      </div>
      <div class="container cont-flex">

        <ul class="grid">
          <!-- <li v-for="(comic,i) in comics" :key="i" class="card">
            <div class="comic-image">
              <img class="comic-image" :src="comic.thumb" alt="">
            </div>
            <h3 class="card-title">{{ comic.series }}</h3>
          </li> -->

          <!-- 3... stampare e ciclare il componente CArd------------------------------>
          <Card v-for="(comic,i) in comics" :key="i" :thumb="comic.thumb" :series="comic.series"  />
        </ul>
        
      </div>

        <div class="container">
          <div class="load-button">
            <button class="custom-button">LOAD MORE</button>
          </div>

        </div>

      </div>
    </section>
  </main>
</template>


<style lang="scss" scoped>


.cont-flex{
  display: flex;
  justify-content: center;
}

.load-button{
  display: flex;
  justify-content: center;
}
.custom-button{
  background-color: #0282F9;
  border-radius: 0px;
}

  .container-griglia{
    position: relative;
  }
  .current-series{
    padding: 10px;
    background-color: #0282F9;
    position: absolute;
    top: -75px;
    left: 10px;
  } 
    h3{
      font-size: 28px;
    }

  section{
    background-color: #1C1C1C;
    min-height: 140px;
  }
  
  .grid-sect{
    padding: 40px 0px;
  }

  .grid{
    display: grid;
    grid-template-columns: repeat(6,1fr);
    gap: 10px;
    
  }
    
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
  .hero-immagine{
    background-image: url('/images/jumbotron.jpg');
    min-height: 450px;
    position: relative;
    background-repeat: no-repeat;
    background-size: cover;
  }


</style>