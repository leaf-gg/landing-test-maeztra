<template>
<header>
  <div class="topbar">
          <p>
            Acompanhe as melhores promoções disponíveis aqui na Maeztra.
          </p>
      </div>
    <div class="shell">
          <div class="mobile-header" v-if="isMobile">
              <div>
            <i class="menu"></i>
                <i class="logo-mobile"></i>
            </div>
            <div class="header-buttons">
                <i class="search"></i>
            <i class="wishlist"></i>
            </div>
          </div>
            </div>
          <div class="desktop-header" v-if="!isMobile">
            <div class="shell">
            <div class="header-content">
              <div class="logo">
                <a href="#">
                  <i class="logo-desktop"></i>
                </a>
              </div>
              <div>
              <form action="get">
                <input type="text" placeholder="O que você busca?" required>
                <button type="submit" class="btn-default">Buscar</button>
              </form>
              </div>
              <div class="options">
                  <a href="">
                    <i class="account"></i>
                    Minha Conta
                  </a>

                  <a href="">
                    <i class="heart"></i>
                    Lista de Desejos
                  </a>

                <a href="" class="cart">
                  <i class="bag"></i>
                  Meu Carrinho
                </a>

              </div>
            </div>
            </div>
            <nav class="nav-options">
             <div class="shell">
              <ul>
                <li><a href=""><i class="new"></i>Novidades</a></li>
                <li><a href="">Vestidos</a></li>
                <li><a href="">Roupas</a></li>
                <li><a href="">Sapatos</a></li>
                <li><a href="">Lingerie</a></li>
                <li><a href="">Acessórios</a></li>
                <li><a href="">OUTLET</a></li>
              </ul>
              </div>
            </nav>
          </div>
  
</header>
</template>

<script>
export default {
    data() {
        return {
            isMobile: window.screen.width <= 767,
        };
    }
}
  </script>
<style lang="scss">

@import '../assets/styles/main.scss';
header{ 
  background: $white;
  box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.08);

  @include media(mobile){
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 10;
  }

  .topbar{
    background: $black;
    color: $white;
    width: 100%;
    height: 24px;
    @include fontRegular(10px);
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 3px 0;

    @include media(desktop){
    @include fontRegular(12px);

    }
  }
  .mobile-header{ 
      width: 100%;
      height: 88px;
      padding: 35px 20px;
      display: flex;
      justify-content: space-between;
}
.desktop-header{
  .header-content{
    width: 100%;
    height: 88px;
    padding: 35px 0px;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .logo{
     width: 93px;
    }

      form{
        width: 672px;
        input{
          width:  671px;
          border-radius: 10px;
          background: $border;
          height: 40px;
          padding-left: 24px;
          padding-right: 130px;
          border: none;
        }
        button{
          width: 119px;
          height: 40px;
          margin: 0 -119px;
          padding: 7px;
        }
      }

      .options{
        display: flex;
        width: 422px;
        justify-content: space-between;
        align-items: center;
        a{
          @include fontRegular(14px);
          line-height: 21px;
          color: $black-2;
        }

           .cart{
            border: 1px solid $orange;
            border-radius: 4px;
            padding: 6px;
          }
      }
  }
  .nav-options{
    padding: 13px;
   box-shadow: inset 0px 4px 6px 0px rgba(0, 0, 0, 0.08);
    background: $white;
    margin: 0 auto;
    width: 100%;

    ul{
      width: 100%;
      display: flex;
      justify-content: space-between;
      padding: 0 150px;

      
      li{

        a{
         @include fontRegular(14px);
         line-height: 21px;
         color: $black-2; 
        }
      }
    }
  }
}
}
</style>