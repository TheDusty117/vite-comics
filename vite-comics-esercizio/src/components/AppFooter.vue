<script>

export default {
  data(){
    return {

      menu1:{
        title: 'dc comics',
        links: [
          'Characters',
          'Comics',
          'Movies',
          'TV',
          'Games',
          'Videos',
          'News',
        ]
      },

      menu2:{
        title: 'dc',
        links: [
          'Termis Of Use',
          'Privacy policy(New)',
          'Ad Choices',
          'Advertising',
          'Jobs',
          'Subscriptions',
          'Talent Workshops',
          'CPSC Certificates',
          'Ratings',
          'Shop Help',
          'Contact Us',

        ]
      },

      menu3:{
        title: 'sites',
        links: [
          'DC',
          'MAD Magazine',
          'DC Kids',
          'DC Universe',
          'DC Power Visa',
        ]
      },

    }
  }
}
</script>


<template>
  <footer>

    <section class="bg-comics">
      <div class="container">

        <!--riga dei link con background-->
        <div class="row row-infos">

          <div class="row row-links">

            <!--menu 1-->
            <ul class="infos-list">

              <h2>{{ menu1.title }}</h2>
              <li v-for="link in menu1.links" key="i" class="infos-item">
                <a href="">{{ link }}</a>
              </li>
              
            </ul>

            <!--menu 2-->
            <ul class="infos-list">

              <h2>{{ menu2.title }}</h2>
              <li v-for="link in menu2.links" key="i" class="infos-item">
                <a href="">{{ link }}</a>
              </li>
              
            </ul>

            <!--menu 3-->
            <ul class="infos-list">

              <h2>{{ menu3.title }}</h2>
              <li v-for="link in menu3.links" key="i" class="infos-item">
                <a href="">{{ link }}</a>
              </li>
              
            </ul>
          </div>

          <div class="col-logo">
            <img class="dc-big" src="/images/dc-logo-bg.png" alt="">
          </div>

        </div>

      </div>
    </section>


    <!--SEZIONE SOCIAL--------------------------->
    <section class="section-socials">

      <div class="container">

        <div class="row row-socials">

          <div class="col-button">
            <button class="sign-button">
              sign-up now!
            </button>
          </div>

          <div class="col-socials">
            <ul class="row social-list">
              <h3 class="follow">follow us</h3>
              <li class="social-item">
                <img src="/images/footer-facebook.png" alt="">
              </li>
              <li class="social-item">
                <img src="/images/footer-twitter.png" alt="">
              </li>
              <li class="social-item">
                <img src="/images/footer-youtube.png" alt="">
              </li>
              <li class="social-item">
                <img src="/images/footer-pinterest.png" alt="">
              </li>
              <li class="social-item">
                <img src="/images/footer-periscope.png" alt="">
              </li>
            </ul>
          </div>

          
        </div>

      </div>

    </section>

  </footer>
</template>


<style lang="scss" scoped>

.row-infos{
  justify-content: space-between;
}

.row-links{
  justify-content: space-evenly;
  gap: 30px;
}
  .infos-list{
    width: 140px;
    padding-top: 30px;
  }

  .infos-item{
    font-size: 15px;
    color: gray;
  }

  h2{
    text-transform: uppercase;
    font-size: 20px;
  }

.dc-big{
  
}

.bg-comics{
  background-image: url('/images/footer-bg.jpg');
  background-size: cover;
  
}

//                   PARTE DELLO STILE DEI SOCIAL


.section-socials{
  height: 150px;
}
.row-socials{
  justify-content: space-between;
  align-items: center;
  height: 150px;
  
}

.social-list{
  display: flex;
  gap: 20px;
}


.col-button{
  
}

.col-socials{

}

.sign-button{
  padding: 20px 30px;
  text-transform: uppercase;
  border: 2px solid #0282F9;
  border-radius: 0px;
}

.follow{
  text-transform: uppercase;
  color: #0282F9;
}

</style>