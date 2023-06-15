<script >


export default{
  name: "PageFooter",
   props:{
        links:Array,
    }
}

</script>

<template>


      <footer id="footer">

        <div class="container">

            <div class="address">

                <h5>ADDRESS</h5>
                <div class="location"> 382 NE 181st # 87394 Miami, FL 33179-3899</div>
                <div  class="location">+1(305) 547-9909 (9am - 5pm EST, Monday _ Friday)</div>
                <div  class="location"> support@maxcoach.com</div>

                <div>
                    <i class="bi bi-twitter"></i>
                    <i class="bi bi-facebook"></i>
                    <i class="bi bi-instagram"></i>
                    <i class="bi bi-linkedin"></i>
                </div>

            </div>

            <div class="links">

              <div class="title">

                <h5>Explore</h5>
                <h5>Information</h5>

              </div>

                <ul>
                  <li  v-for='(link, index) in links[1].NavMenu' :key='index'>
                      
                      <a href="#"> {{ link }}</a>

                  </li>
                </ul>

                <div class="copyright"> © 2020 MaxCoach, All rights Reserved</div>

                <a class="arrow" href="#top"><i class="bi bi-arrow-up"></i></a> 

            </div>

        </div>


      </footer>

</template>

<style lang="scss" scoped>

@use"../styles/partials/variables.scss" as*;
@use"../styles/general.scss" as*;


footer{
  width: $width;
  min-height: 300px;
  background-color: $black;
  position: relative;

  .container{
    @include container;
    @include flexContent;
    padding: $padding;
    color: $lightgrey;

    .address{
      font-size: $fontLittleSize;
      width: 30%;
      min-height: 300px;
    
      h5{
        color: $white;
        margin: 20px 0;
      }

      .location{
        margin-bottom: 20px;
      }

      i{
        font-size: 25px;
        margin-right: 15px;

        &:hover{
          color: $blue;
        }
      }
      
    }

    .links{
      width: 30%;

      .title{

        h5{
          display: inline;
          color: $white;
          margin-right: 110px;
        }
       
      }

      ul{
          @include flexContent;
          flex-wrap: wrap;

          li{
            margin-top: 8px;
            a{
              padding-right: 20px;
              color: $grey;

              &:hover{
                color: $blue;
              }
            }
          }
        }
    }

  }

 
  .copyright{
          @include flexContent;
          justify-content: center;
          margin-top: 30px;
          color: $grey;;
        }

    .arrow{
      position: absolute;
      padding: 10px 15px;
      background-color: $green;
      border-radius: 50%;
      bottom:10px;
      right: 10px;

      &:hover{
        background-color: $blue;
      }

      i{
        font-size: 24px;
        color: $white;
      }
    }

}


</style>