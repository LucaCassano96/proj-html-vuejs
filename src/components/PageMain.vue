<script >


export default {
    name: "PageMain",
}

</script>

<template>

        <!-- ABOUT ME -->

    <section >
       
        <div id="about_me"> 

            <div class="title">
                <h5>ABOUT ME</h5>
                <h2>How to be an Alpha Male: The 15 Habits of True Alpha</h2>
            </div>

            <div class="description"> 
                <h5>Want to learn how to be <span> <a href="#">an alpha male?</a></span> How to be masculine? How to be the man you've always wanted to be?</h5>
                
                <p>Your goal is to show the consistency of buisness, core values, and customer care. Punctuality, responsability, individuality, accuracy, enthusiasm - you have to clearly explain how these qualities are applicble to your work. And the important thing is you do love what you do.</p>
            </div>
            
        </div> 

        <div id="about_me_presentation">

            <div class="video">
                <iframe 
                
                width="585" height="398" src="https://www.youtube.com/embed/vLFxOOEyhUE" title="Being your Own Life Coach | John Muldoon | TEDxShanghaiAmericanSchoolPuxi" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen>

                </iframe>
            </div>

            <div class="video_description">

                <h3>
                    "Every Morning you have two choices: continue to sleep with your dreams, or wake up and chase them."
                </h3>

                <img src="src\assets\images\home-movation-shape-01.png" alt="waves shape">

                <h4>Kaixa Stark </h4>

                <div>WINGMAN</div>

            </div>

        </div>


    </section>
   
</template>

<style lang="scss" scoped>
@use"../styles/partials/variables.scss" as*;
@use"../styles/general.scss" as*;


    /* ABOUT ME  */

#about_me{

    @include container;
    margin-top: 80px;
    padding: $padding;
    @include flexContent;

    .title{

        width: 40%;

        h5{
        color: $green;
        font-size: 14px;
            
        }

        h2{
            font-size: 40px;
            color: $black;
            font-weight: 400;
            margin-top: 30px;
        }
    }

    .description{
        width: 40%;

        h5{

            font-size: 14px;
            margin: 100px 0 20px 0;
            line-height: 2;
            
            
            span a{
            color: $green;
                &:hover{
                    color: $blue;
                }
            }
        }

        p{
            font-size: 14px;
        }

        
    }

}
/* ABOUT ME Presentation */
#about_me_presentation{
    @include container;
    margin-top: 30px;
    padding: $padding;
    @include flexContent;

    .video{
        width: 60%;
    }

    .video_description{
        width: 35%;

        h3{
            font-size: 30px;
            color: $black;
            font-weight: 400;
        }

        img{
            margin-top: 50px;
        }

        h4{
            font-size: 16px;
            color: $black;
            margin: 30px 0;
        }

        div{
            font-size: 10px;
            color: $grey;
        }
    }
}

</style>