<template>
    <section id="products">
        <h3>As Mais Pedidas</h3>
      <div class="shell">
        <VueSlickCarousel v-bind="settings">
            <div class="product-item">
                <img src="https://via.placeholder.com/308x381" alt="">
                  <div class="product-colors">
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                  </div>
                  <div class="product-description">
                    <p class="price">R$ 500,00</p>
                    <p class="name">Faux Suede Mini Skirt</p>
                    <p class="desc"> A faux suede mini skirt featuring exposed button-front closures and panel seam construction.</p>
                    <button class="btn-default add">Adicionar</button>
                  </div>    
            </div>

            <div class="product-item">
                <img src="https://via.placeholder.com/308x381" alt="">
                  <div class="product-colors">
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                  </div>
                  <div class="product-description">
                    <p class="price">R$ 500,00</p>
                    <p class="name">Faux Suede Mini Skirt</p>
                    <p class="desc"> A faux suede mini skirt featuring exposed button-front closures and panel seam construction.</p>
                    <button class="btn-default add">Adicionar</button>
                  </div>    
            </div>

            <div class="product-item">
                <img src="https://via.placeholder.com/308x381" alt="">
                  <div class="product-colors">
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                  </div>
                  <div class="product-description">
                    <p class="price">R$ 500,00</p>
                    <p class="name">Faux Suede Mini Skirt</p>
                    <p class="desc"> A faux suede mini skirt featuring exposed button-front closures and panel seam construction.</p>
                    <button class="btn-default add">Adicionar</button>
                  </div>    
            </div>

            <div class="product-item">
                <img src="https://via.placeholder.com/308x381" alt="">
                  <div class="product-colors">
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                  </div>
                  <div class="product-description">
                    <p class="price">R$ 500,00</p>
                    <p class="name">Faux Suede Mini Skirt</p>
                    <p class="desc"> A faux suede mini skirt featuring exposed button-front closures and panel seam construction.</p>
                    <button class="btn-default add">Adicionar</button>
                  </div>    
            </div>

                <div class="product-item">
                <img src="https://via.placeholder.com/308x381" alt="">
                  <div class="product-colors">
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                  </div>
                  <div class="product-description">
                    <p class="price">R$ 500,00</p>
                    <p class="name">Faux Suede Mini Skirt</p>
                    <p class="desc"> A faux suede mini skirt featuring exposed button-front closures and panel seam construction.</p>
                    <button class="btn-default add">Adicionar</button>
                  </div>    
            </div>

                <div class="product-item">
                <img src="https://via.placeholder.com/308x381" alt="">
                  <div class="product-colors">
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                  </div>
                  <div class="product-description">
                    <p class="price">R$ 500,00</p>
                    <p class="name">Faux Suede Mini Skirt</p>
                    <p class="desc"> A faux suede mini skirt featuring exposed button-front closures and panel seam construction.</p>
                    <button class="btn-default add">Adicionar</button>
                  </div>    
            </div>

                <div class="product-item">
                <img src="https://via.placeholder.com/308x381" alt="">
                  <div class="product-colors">
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                  </div>
                  <div class="product-description">
                    <p class="price">R$ 500,00</p>
                    <p class="name">Faux Suede Mini Skirt</p>
                    <p class="desc"> A faux suede mini skirt featuring exposed button-front closures and panel seam construction.</p>
                    <button class="btn-default add">Adicionar</button>
                  </div>    
            </div>
                 </VueSlickCarousel>
      </div>
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
                slidesToShow: 5,
                autoplay: false,
                infinite: true,
                slidesToScroll: 1,
                responsive: [
                    {
                        breakpoint: 767,
                        settings: {
                              dots: false,
                            arrows: false,
                            slidesToShow: 1,
                            autoplay: true,
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

#products{
  margin-bottom: 80px;

    h3{
    @include fontBold(24px);
    text-align: center;
    margin: 80px 0 24px;
  }
  .product-item{
    width: 100%;
    padding: 10px;

    @include media(desktop){
      padding-left: 14px;
      padding-right: 0;
    }
    img{
      width: 100%;
    }
    
  }

  .product-colors{
    display: block;
    margin: 23px 0;
    span{

    padding: 2px 13px;
      border-radius: 4px;
      background: $orange;
      margin: 0 4px;
    &:first-of-type{
      margin-left: 0;
    }

  &:nth-child(2){
      background: #D37164;
    }

    &:nth-child(3){
      background: #6497D3;
    }
    &:nth-child(4){
      background: #3C3B79;
    }
    
    }
  }
.product-description{
  margin-bottom: 20px;
  .price{
    @include fontBold(20px);
    color: $black-2;
    line-height: 30px;
    margin-bottom: 2px;
  }
  .name{
    @include fontRegular(16px);
    line-height: 24px;
    color: $black-2;
    margin-bottom: 8px;
  }

  .desc{
    @include fontRegular(12px);
    color: $black-2;
    line-height: 18px;
    opacity: .5;
    margin-bottom: 8px;
  }

  .add{
    width: 100%;
  }

}

}
</style>