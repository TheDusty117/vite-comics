<script>
export default {
  data(){
    
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
            <ul class="infos-list">
              <h2>dc comics</h2>
              <li class="infos-item">
                <a href="">Characters</a>
              </li>
              <li class="infos-item">
                <a href="">Comics</a>
              </li>
              <li class="infos-item">
                <a href="">Movies</a>
              </li>
              <li class="infos-item">
                <a href="">TV</a>
              </li>
              <li class="infos-item">
                <a href="">Games</a>
              </li>
              <li class="infos-item">
                <a href="">Videos</a>
              </li>
              <li class="infos-item">
                <a href="">News</a>
              </li>

              <h2>
                Shop
              </h2>
              <li class="infos-item">
                <a href="">Shop DC</a>
              </li>
              <li class="infos-item">
                <a href="">Shop DC Collectibles</a>
              </li>
              
            </ul>

            <ul class="infos-list">
              <h2>dc</h2>
              <li class="infos-item">
                <a href="">Terms Of Use</a>
              </li>
              <li class="infos-item">
                <a href="">Privacy policy(New)</a>
              </li>
              <li class="infos-item">
                <a href="">Ad Choices</a>
              </li>
              <li class="infos-item">
                <a href="">Advertising</a>
              </li>
              <li class="infos-item">
                <a href="">Jobs</a>
              </li>
              <li class="infos-item">
                <a href="">subscriptions</a>
              </li>
              <li class="infos-item">
                <a href="">Talent Workshops</a>
              </li>
              <li class="infos-item">
                <a href="">CPSC Certificates</a>
              </li>
              <li class="infos-item">
                <a href="">Ratings</a>
              </li>
              <li class="infos-item">
                <a href="">Shop Help</a>
              </li>
              <li class="infos-item">
                <a href="">Contact Us</a>
              </li>
            </ul>

            <ul class="infos-list">
              <h2>sites</h2>
              <li class="infos-item">
                <a href="">DC</a>
              </li>
              <li class="infos-item">
                <a href="">MAD Magazine</a>
              </li>
              <li class="infos-item">
                <a href="">DC Kids</a>
              </li>
              <li class="infos-item">
                <a href="">DC Universe</a>
              </li>
              <li class="infos-item">
                <a href="">DC Power Visa</a>
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