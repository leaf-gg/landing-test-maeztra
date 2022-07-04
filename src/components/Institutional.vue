<template>
  <section id="institutional">
    <div class="shell">
        <div class="contents">
            <div class="content">
              <h4>Lorem ipsum</h4>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Interdum mauris posuere fusce proin mattis. Hendrerit cras ut nunc enim dictum. Mattis proin ut quis donec sed eget nulla. Vel mi ut mauris integer. Nibh sagittis in lobortis sed cursus condimentum velit pharetra. Amet luctus ut vulputate scelerisque .
              </p>
            </div>
            <div class="content">
              <img src="https://i.imgur.com/1vLCv01.png">

            </div>
        </div>
    </div>
 
  </section>
</template>

<style lang="scss">
@import '../assets/styles/main.scss';
  #institutional{
    .contents{

      @include media(desktop){
        display: flex;
        justify-content: space-between;
      }
      .content{
        padding-right: 40px;
          @include media(desktop){
            display: flex;
            flex-direction: column;
            align-self: center;
            width: 23%;
            margin-right: 64px;
            padding: 0;
          }
        &:last-of-type{
          padding: 0;
                @include media(desktop){
                      width: 60%;
                      margin: 0;
                    }
        }
        h4{
          @include fontBold(24px);
          color: $black;
          line-height: 37px;
          margin-bottom: 16px;
        }

        p{
          @include fontRegular(14px);
          color: $black;
          line-height: 21px;
          margin-bottom: 24px;
        }
        img{
          margin-bottom: 39px;
          border-radius: 4px;
            @include media(desktop){
              width: 1114px;
            }

        }
      }
    }
  }

</style>