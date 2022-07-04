<template>
<section id="brands">
  <div class="shell">
        <h3>Marcas Parceiras</h3>
        <div class="brands-boxes">
          <div class="brand-box">
              <img src="https://i.imgur.com/JOTNQgl.png">
          </div>

             <div class="brand-box">
              <img src="https://i.imgur.com/JOTNQgl.png">
          </div>

             <div class="brand-box">
              <img src="https://i.imgur.com/JOTNQgl.png">
          </div>

             <div class="brand-box">
              <img src="https://i.imgur.com/JOTNQgl.png">
          </div>



             <div class="brand-box">
              <img src="https://i.imgur.com/JOTNQgl.png">
          </div>

          </div>
         </div>
  </section>
</template>
<style lang="scss">
@import '../assets/styles/main.scss';
#brands{

  h3{
    @include fontBold(24px);
    text-align: center;
    margin: 21px 0 24px;
  }

  .brands-boxes{
display: flex;
	flex-wrap: nowrap;
	overflow-x: scroll;

  @include media(desktop){
    overflow: hidden;
  }
   
    .brand-box{
      width: 308px;
      height: 64px;
      display: contents;
      margin-right: 20px;

      @include media(desktop){
        display: inherit;

        &:last-of-type{
             margin: 0;
     
        }
      }

    img{
      margin-right: 20px;
    }

    }
    }
}
</style>