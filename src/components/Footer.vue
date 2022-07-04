<template>
  <footer>
      <div class="newsletter">
        <p>Receba Nossa Newsletter</p>
        <form action="get">
                <input type="text" placeholder="Digite seu e-mail" required>
                <button type="submit" class="btn-default">Enviar</button>
          </form>
      </div>

          <div class="shell">
         <div class="accordions">
          <div class="accordion-item">
              <input type="radio" name="accordion" id="accordion-1">
              <label for="accordion-1">Informações</label>
              <div class="accordion-content">
                <ul>
                  <li><a href="">Quem somos</a></li>
                  <li><a href="">Prazo de Envio</a></li>
                  <li><a href="">Trocas e Devoluções</a></li>
                  <li><a href="">Promoções e Cupons</a></li>
                </ul>
              </div>
          </div>

             <div class="accordion-item">
              <input type="radio" name="accordion" id="accordion-2">
              <label for="accordion-2">Minha Conta</label>
              <div class="accordion-content">
                <ul>
                  <li><a href="">Minha Conta</a></li>
                  <li><a href="">Meus Pedidos</a></li>
                  <li><a href="">Cadastre-se</a></li>
        
                </ul>
              </div>
          </div>

             <div class="accordion-item">
              <input type="radio" name="accordion" id="accordion-3">
              <label for="accordion-3">Onde nos Encontrar</label>
              <div class="accordion-content">
                <ul>
                  <li><a href="">Lojas</a></li>
                  <li><a href="">Endereço</a></li>
                </ul>
              </div>
          </div> 
          </div>
    </div>
    <div class="copyright">
   
          <div class="shell">
        <div class="copyright-items">
        <div class="social">
        <a href="">      <i class="facebook"></i></a>
        <a href="">   <i class="linkedin"></i></a>
        <a href="">    <i class="instagram"></i></a>
        <a href="">   <i class="youtube"></i></a>
        </div>
        <div class="cards">
          <i class="visa"></i>
          <i class="master"></i>
          <i class="visa"></i>
          <i class="master"></i>
        </div>
        <div class="authors">
          <a href="#">
            Powered By
            <i class="vtex"></i>
          </a>

          <a href="#">Developed by
                <i class="maeztra"></i>
          </a>
        
        </div>  
        </div>
        </div>
   
    </div>
  </footer>
</template>

<style lang="scss">
@import '../assets/styles/main.scss';

.newsletter{
  background: $lightgray;
  border: 1px solid $border;
  height: 120px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
  margin-bottom: 40px;

  @include media(desktop){
    flex-direction: row;
    align-items: center;

  }

p{
  @include fontBold(24px);
  line-height: 37px;
  color: $black-2;
  margin-bottom: 8px;
  @include media(desktop){
    margin-right: 30px;
    margin-bottom: 0;
  }
}

input{
  padding-left: 24px;
  @include fontRegular(14px);
  line-height: 21px;
  border: 1px solid $black-2;
  border-radius: 4px;
  width: 204px;
  height: 26px;
  margin-right: 15px;

  @include media(desktop){
    width: 630px;
    height: 40px;
    margin-right: -10px;
  }
}
button{
  width: 79px;
  height: 26px;
  @include fontBold(14px);
  line-height: 21px;
  padding: 0;

  @include media(desktop){
    width: 131px;
    height: 40px;
  }
}
}

.accordions{
  margin-bottom: 56px;
  display: flex;
  flex-direction: column;

  @include media(desktop){
    flex-direction: row;
    justify-content: space-between;
    padding: 0 150px;
  }

  a{
    color: $black;
    @include fontRegular(12px);
    margin-bottom: 24px;
  }

  label{
    display: block;
    @include fontBold(16px);
    line-height: 18px;
    color: $black-2;
    margin-bottom: 17px;
  }
  input{
    opacity: 0;
  }
  .accordion-content{
    display: none;

    @include media(desktop){
      display: block;
    }
  }
}
.copyright{
  background: $black-2;
  height: 233px;
  padding: 28px 0;
  display: flex;
  justify-content: center;
  align-self: center;

  @include media(desktop){
    width: 100%;
    height: 85px;

    .shell{
      width: 100%;
      margin: 0;
    }
  }
  

  .copyright-items{
    width: 100%;
    margin: 0 auto;
    @include media(desktop){
      display: flex;
      justify-content: space-between;
    }
  }

.social{
  margin-bottom: 36px;
}
.cards{
  margin-bottom: 45px;
}
  .social, .cards{
    text-align: center;

    @include media(desktop){
      margin: 0;
    }

    a{  
          margin-right: 24px;
      &:last-of-type{
        margin: 0;
      }
  
    }

      i{
          margin-right: 24px;
      &:last-of-type{
        margin: 0;
      }
  
    }
  }

  .authors{
    display: flex;
    margin: 0 auto;
    justify-content: center;

    @include media(desktop){
      margin: 0;
    }
  
    a{
      @include fontRegular(10px);
      line-height: 14px;
      color: $white;
      margin-bottom: 4px;
      display: flex;
      flex-direction: column;
      
    }
  }
}
</style>