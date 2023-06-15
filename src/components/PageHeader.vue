<script >
import NavBarMenu from './NavBarMenu.vue'
import PageFooter from "./PageFooter.vue"
import PageMain from './PageMain.vue'

export default{
  name: "PageHeader",
  components:{
    NavBarMenu,
    PageMain,
    PageFooter
  },
  data(){
    return{
        menu:[
            {
                navEl: "Home",
                NavMenu:["Our Story","Projects","Products","Work with us", "Terms of Service"]
            },
            {
                navEl: "Pages",
                NavMenu:["Start Here","Success Story","Membership", "Courses", "Purchase guide", "About Us", "Contact US", "provacy policy", "Terms of service"]
            },
            {
                navEl: "Courses",
                NavMenu:["Blue Planet","Motivation","live better","help others", "No pain no gain", "skills for the future"]
            },
            {
                navEl: "Features",
                NavMenu:["With you everyday","FAQ","Contact Us","Second page"]
            },
            {
                navEl: "Blog",
                NavMenu:["Blog","Facebook","TikTok","Linkedin"]
            },
            {
                navEl: "Shop",
                NavMenu:["Our Products","Start for free","Paly with me"]
            },
        ]
    }
  }
}

</script>

<template>
 
    <Header>

        <div id="container">

            <nav>
                <NavBarMenu :links="menu"/>
            </nav>

            <div id="jambo">

                <div class="jambo_description">
                    <h5>I'M WINGMAN</h5>
                    <h1>Peace On Earth A Wonderful Wish But No Way</h1>
                    <p>Sucess is not overnight. It's when everyday you get a little better then the day before.It all adds up</p>
                    <a href="#">Get started for free <i class="bi bi-arrow-right"></i></a>
                </div>

                <div class="jambo_img">
                    <img src="src\assets\images\home-movation-hero-image.png" alt="home-movation-hero">
                </div>

        
            </div>

            <div class="data">

                <div>
                    <div class="number">1.926</div>
                    <div class="number_description">FINISHED SESSION</div>
                </div>

                <div>
                    <div class="number">100%</div>
                    <div class="number_description">SATISFACTION RATE</div>
                </div>

                <div>
                    <div class="number">3092+</div>
                    <div class="number_description">ENROLLED LEARNERS</div>
                </div>

                <div>
                    <div class="number">200</div>
                    <div class="number_description">ONLINE INSTRUCTORS</div>
                </div>

            </div>


        </div>

        <div class="tools">
            <a href="#"><i class="bi bi-rulers"></i></a>
            <a href="#"><i class="bi bi-wrench-adjustable-circle-fill"></i></a>
            <a href="#"><i class="bi bi-journal-bookmark-fill"></i></a>
            <a href="#"><i class="bi bi-cart"></i></a>
                    
        </div>
        
    </Header>
    
    <PageMain/>
    <PageFooter :links="menu"/>

</template>

<style lang="scss" scoped>

@use"../styles/partials/variables.scss" as*;
@use"../styles/general.scss" as*;


/* HEADER */

header{
    width: $width;
    min-height: 300px;
    background-image: url("src/assets/images/abstract-wavy-smooth-lines-pattern-free-vector-2.jpg");
    object-fit: cover;
    position: relative;

    #container{
        @include container;
        min-height: 300px;

        nav{
            width: $width;
            height: 80px;
        }

        #jambo{
            margin-top: 50px;
            width: $width;
            min-height: 300px;
            display: $displayflex;

            .jambo_description{
                width: $halfwidth;
                min-height: 300px;
                padding: $padding;

                h5{
                    font-size: $fontLittleSize;
                    margin-bottom: 15px;
                    color: $black;
                }

                h1{
                    font-size: 58px;
                    font-weight: 400;
                    color: $black;
                }

                p{
                    color: $black;
                    margin: 50px 0;
                }

                a{
                    @include buttom;

                    i{
                        margin-left: 10px;
                    }
                }
               
                
            }
            .jambo_img{
                width: $halfwidth;
                min-height: 300px;
                padding: 20px;
                
                img{
                    width: $width;
                    object-fit: cover;
                    background-image: url("src/assets/images/home-movation-shape-face-600x534.png"); 
                    background-size: cover; 

                }
            }


        }

        .data{
            margin-top: 60px;
            @include flexContent;
            text-align: center;
            padding: $padding;

            .number{
                color: $green;
                font-size: $fontMediumSize;
                font-weight: 700;
            }

            .number_description{
                font-size: $fontLittleSize;
            }
        }
    }

    .tools{
        position: absolute;
        right: 0;
        top: 30%;
        width: 30px;
        min-height: 100px;
        background-color: $white;
        box-shadow: $shadow;

        a{
            display: block;
            padding: 5px;

            i{
                font-size: $fontMediumSize;
                padding: 10px 0;
                color: $grey;
                
                &:hover{
                color: $blue;
                }
            }
        }



    }

}

</style>