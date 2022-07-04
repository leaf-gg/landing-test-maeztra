<template>
<section id="benefits">
  <div class="shell">
        <h2>Por que comprar na Maeztra?</h2>
        <div class="benefits-boxes">
          <div class="benefit-box">
              <img src="https://i.imgur.com/QTFwPmU.png">
              <div class="content-box">
                <p><strong>Produtos Importados</strong></p>
                <p>Produto de Alta Qualidade</p>
              </div>
          </div>

            <div class="benefit-box">
              <img src="https://i.imgur.com/QTFwPmU.png">
              <div class="content-box">
                <p><strong>Produtos Importados</strong></p>
                <p>Produto de Alta Qualidade</p>
              </div>
          </div>

            <div class="benefit-box">
              <img src="https://i.imgur.com/QTFwPmU.png">
              <div class="content-box">
                <p><strong>Produtos Importados</strong></p>
                <p>Produto de Alta Qualidade</p>
              </div>
          </div>

          <div class="benefit-box">
              <img src="https://i.imgur.com/QTFwPmU.png">
              <div class="content-box">
                <p><strong>Produtos Importados</strong></p>
                <p>Produto de Alta Qualidade</p>
              </div>
          </div>
          </div>
         </div>
  </section>
</template>
<style lang="scss">
@import '../assets/styles/main.scss';
#benefits{
  margin-bottom: 74px;

  h2{
    @include fontBold(16px);
    text-align: center;
    margin: 21px 0 24px;
  }

  .benefits-boxes{
    overflow-x: auto;
    overflow-y: hidden;
    white-space: nowrap;
    display: flex;

    .benefit-box{
      background: $gray;
      padding: 16px 42px;
      width: 308px;
      height: 64px;
      border-radius: 4px;
      display: flex;
      align-content: center;
      align-items: center;
      margin-right: 20px;
      padding-right : 70px;

      @include media(desktop){
        width: 25%;

        &:last-of-type{
          margin-right: 0;
        }
      }
    img{
      margin-right: 21px;
    }
      p{
          line-height: 18px;
      }
    }
    }
}
</style>