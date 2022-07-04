<template>
  <section id="banners">

    <VueSlickCarousel v-bind="settings">
    <div class="banner-item">
        <div class="shell">
          <div class="banner-content">
                   <h1>Promoções de Outono</h1>
                <p>Confiras os melhores looks para combinar com você nesse Outono</p>
              <a class="btn-default" href="#">Conferir</a>
          </div>
        </div>
        <img src="https://i.imgur.com/ftECh3G.png">
    </div>
     <div class="banner-item">
        <div class="shell">
          <div class="banner-content">
                   <h1>Lorem ipsum</h1>
                <p>Confiras os melhores looks para combinar com você nesse Outono</p>
              <a class="btn-default" href="#">Conferir</a>
          </div>
        </div>
        <img src="https://i.imgur.com/ftECh3G.png">
    </div>
      <div class="banner-item">
        <div class="shell">
          <div class="banner-content">
                   <h1>Promoções de Outono</h1>
                <p>Confiras os melhores looks para combinar com você nesse Outono</p>
              <a class="btn-default" href="#">Conferir</a>
          </div>
        </div>
        <img src="https://i.imgur.com/ftECh3G.png">
    </div>
     <div class="banner-item">
        <div class="shell">
          <div class="banner-content">
                   <h1>Lorem ipsum</h1>
                <p>Confiras os melhores looks para combinar com você nesse Outono</p>
              <a class="btn-default" href="#">Conferir</a>
          </div>
        </div>
        <img src="https://i.imgur.com/ftECh3G.png">
    </div>
    </VueSlickCarousel>

  </section>
</template>
<script>
 import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'

export default {
    data() {
        return {

settings: {
                arrows: true,
                dots: true,
                slidesToShow: 1,
                autoplay: false,
                infinite: true,
                slidesToScroll: 1,
                responsive: [
                    {
                        breakpoint: 767,
                        settings: {
                              dots: true,
                            arrows: true,
                            slidesToShow: 1,
                            autoplay: false,
                            infinite: true,
                            slidesToScroll: 1,
                        },
                    },
                ],
            },
        };
    },
    components: { VueSlickCarousel },
    created() {},
    methods: {},
};
</script>
<style lang="scss">
@import '../assets/styles/main.scss';
#banners{
  @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');
  font-family: 'Montserrat', sans-serif;

      @include media(mobile){
      height: 320px;
      margin-top: 113px;
      img{
        height: 320px;
        object-fit: cover;
      }
    }


@include media(desktop){
  .slick-prev{
    left: 262px;
  }
  .slick-next{
    right: 262px;
  }
}

.slick-arrow{
  @include media(mobile){
    top: 125px;
  }
}

.slick-dots {
    text-align: center;
    position: absolute;
    width: 100%;
    margin: -60px 0;

    li {
        display: inline;
        width: 100%;

        button {
            background: none;
            font-size: 0;
            border: 1px solid $orange;
            appearance: none;
            width: 16px;
            height: 16px;
            cursor: pointer;
            border-radius: 8px;
            margin: 0 5px;

            @include media(mobile){
              width: 8px;
              height: 8px;
            }
        }

        &.slick-active > button {
            background: $orange;
        }
    }
}


  .banner-content{
    position: absolute;
    margin: 150px 0;
    padding-left: 60px;

    @include media(mobile){
      margin: 50px 0;
      padding-left: 40px;
    }
    

    h1{
      font-size: 40px;
      font-weight: 700;
      color: $white;
      line-height: 49px;
      margin-bottom: 40px;

      @include media(mobile){
        font-size: 30px;
        line-height: 37px;
        margin-bottom: 24px;
        width: 200px;
      }
    }
    p{
      font-size: 20px;
      font-weight: 400;
      color: $white;
      width: 450px;
      margin-bottom: 46px;

      @include media(mobile){
        font-size: 14px;
        width: 227px;
        margin-bottom: 26px;
      }
    }
    a{
      border-radius: 10px;
      width: 128px;
      padding: 10px 32px;
    }
  }
}
</style>