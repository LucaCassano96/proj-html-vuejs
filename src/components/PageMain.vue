<script >
import MainCourses from './MainCourses.vue'

export default {
    name: "PageMain",
    components:{
        MainCourses
    },
    data(){
        return{
            courses:[
            {
                img: "src/assets/images/motivation-course-06-480x298.jpg",
                prize: "30",
                description: "How to be Successful: Create A Growth Mindest For Success",
                lessons: 3,
                students: 50,
            },

            {
                img: "src/assets/images/motivation-course-05-480x298.jpg",
                prize: "30",
                description: "How to Build Confidance in Your Abilities",
                lessons: 1,
                students: 50,
            },
            {
                img: "src/assets/images/motivation-course-04-480x298.jpg",
                prize: "20",
                description: "Productivity Machine - Focus in a Distracted World",
                lessons: 5,
                students: 50,
            },
            {
                img: "src/assets/images/motivation-course-03-480x298.jpg",
                prize: "20",
                description: "Effective Time Management Mastery - Complete Guide",
                lessons: 18,
                students: 50,
            },
            {
                img: "src/assets/images/motivation-course-02-480x298.jpg",
                prize: "25.99",
                description: "Body Language Secrets for Entreprneurs",
                lessons: 19,
                students: 50,
            },
            {
                img: "src/assets/images/motivation-course-01-480x298.jpg",
                prize: "19.99",
                description: "Management Skills: The Science of Leadership",
                lessons: 17,
                students: 50,
            },
            ]
        }
    }
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

    <!-- ONLINE COURSES -->

    <section>

        <div class="online_courses_title"> 

            <h5>BEGIN YOUR JOURNEY AT MAX</h5>
            <h2>Latest <span>Online Courses</span></h2>

        </div>

        <div id="online_courses">

            <MainCourses :course="courses"/>
        
        </div>

        <div class="buttom">
            <a href="#">View all courses <i class="bi bi-arrow-right"></i></a>
        </div>


    </section>


    <!-- BOOKS -->

    <section>

        <div id="books">

            <div class="books_description">

                <h5>BOOK STORE ONLINE</h5>
                <h2>Be Alpha With <span>Wigman's Book</span></h2>
                <div class="description"><i class="bi bi-check2"></i> Help you understand yourself better</div>
                <div class="description"><i class="bi bi-check2"></i> Revealing mature tips</div>
                <div class="description"><i class="bi bi-check2"></i> Give the right advice</div>
                <div class="description"><i class="bi bi-check2"></i> Fascinating examples of alpha man</div>
                <div class="Ebook">
                    <a href="#">Get Free Ebook</a>
                </div>
                

            </div>

            <div class="book">

                <img src="src\assets\images\product-book-11-400x400.jpg" alt="book">
                <div class="book_name">Alpha man by MaxCoach </div>
                <div class="book_price">$29.00</div>

                <div class="book_tools">

                    <div class="tool"><a href=""><i class="bi bi-search"></i></a></div>
                    <div class="tool"><a href=""><i class="bi bi-cart-check"></i></a></div>
                    <div class="tool"><a href=""><i class="bi bi-heart"></i></a></div>
                    <div class="tool"><a href=""><i class="bi bi-bar-chart-fill"></i></a></div>

                </div>

            </div>

            <div class="book">

                <img src="src\assets\images\product-book-10-400x400.jpg" alt="book">
                <div class="book_name">Alpha man by MaxCoach </div>
                <div class="book_price">$29.00</div>

                <div class="book_tools">

                    <div class="tool"><a href=""><i class="bi bi-search"></i></a></div>
                    <div class="tool"><a href=""><i class="bi bi-cart-check"></i></a></div>
                    <div class="tool"><a href=""><i class="bi bi-heart"></i></a></div>
                    <div class="tool"><a href=""><i class="bi bi-bar-chart-fill"></i></a></div>

                </div>

            </div>      


        </div>

    </section>

    <!-- BRANDS -->

    <section>

        <div id="brands">

            <div><img src="src\assets\images\client-logo-05-primary.png" alt="sponsor"></div>
            <div><img src="src\assets\images\client-logo-06-primary.png" alt="sponsor"></div>
            <div><img src="src\assets\images\client-logo-07-primary.png" alt="sponsor"></div>
            <div><img src="src\assets\images\client-logo-04-primary.png" alt="sponsor"></div>
            <div><img src="src\assets\images\client-logo-03-primary.png" alt="sponsor"></div>
            <div><img src="src\assets\images\client-logo-02-primary.png" alt="sponsor"></div>



        </div>


    </section>

    <!-- REAL STORIES -->

    <section>

        <div id="real_stories">

            <div class="story_description">

                <div class="description">
                    <h5>REAL STORIES</h5>

                    <p>I am free to learn at my own pace, follow my own schedule and choose the subject i want to learn from the syllabus. Great study portalfor people like me</p>
                    <img src="src\assets\images\testimonial-avata-02.jpg" alt="testimonial">

                    <p>Mina Hollace</p>
                    <div class="profession">/ Freelancer</div>
                </div>
                
            </div>

            <div class="story_img">
                 <img src="src\assets\images\home-movation-testimonial-image-600x439.jpg" alt="testimonial" > 
            </div>

            <div class="buttom_sliders">

                <i class="bi bi-caret-up"></i>
                <div>1/4</div>
                <i class="bi bi-caret-down"></i>

            </div>

        </div>

    </section>

    <!-- ARTICLES -->

    <section>

        <div id="articles">

            <h5>BLOG UPDATED</h5>
            <h2>Interesting <span>articles updated </span> daily</h2>
            <div class="articles_container">

                <div class="article">
                    
                    <img src="src\assets\images\motivation-blog-04-480x325.jpg" alt="motivation-blog">
                    <div class="date"><i class="bi bi-calendar"></i> May 13, 2020</div>
                    <h5>How to Stay True to Your Personal Brand</h5>

                    <p>When it comes to your buisiness or career, you want...</p>

                </div>

                <div class="article">
                    
                    <img src="src\assets\images\motivation-blog-03-480x325.jpg" alt="motivation-blog">
                    <div class="date"><i class="bi bi-calendar"></i> May 13, 2020</div>
                    <h5>5 Vital Lessons in 5 Years of Freelancing</h5>

                    <p>ceing self-employed and working from home, it's easy to get...</p>

                </div>

                <div class="article">
                    
                    <img src="src\assets\images\motivation-blog-02-480x325.jpg" alt="motivation-blog">
                    <div class="date"><i class="bi bi-calendar"></i> May 13, 2020</div>
                    <h5>11 super Useful Tips for Small-Business Owners</h5>

                    <p>being a small-business owner poses a ton of challenges. We...</p>

                </div>

                <div class="article">
                    
                    <img src="src\assets\images\motivation-blog-01-480x325.jpg" alt="motivation-blog">
                    <div class="date"><i class="bi bi-calendar"></i> May 13, 2020</div>
                    <h5>How to Give Yourself Grace to Start Again</h5>

                    <p>Forgive yourself for bad habits you may started or...</p>

                </div>

            </div>

            <a href="#">VIEW ALL POSTS</a>

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
        font-size:$fontLittleSize;
            
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

            font-size: $fontLittleSize;
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
            font-size: $fontLittleSize;
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
            font-size: $fontLittleSize;
            color: $black;
            margin: 30px 0;
        }

        div{
            font-size: 10px;
            color: $grey;
        }
    }
}

 /* ONLINE COURSES  */

.online_courses_title{
    text-align: center;
    margin: 80px 0 50px 0;

    h5{
        font-size:$fontLittleSize;
        color: $grey;
    }

    h2{
        font-size: $fontBigSize;
        color: $blue;
        font-weight: 400;
        margin-top: 20px;

        span{
            color: $green;
        }
    }
}

#online_courses{
    @include container;
    padding: $padding;
    @include flexContent;
    flex-wrap: wrap;

}

.buttom{
    @include flexContent;
    justify-content: center;

    a{
        @include buttom;
        
    }

}


/* BOOKS */

#books{
    @include container;
    margin-top: 80px;
    @include flexContent;
    padding: $padding;
    
    .books_description{
        width: calc(100% / 3);

        h5{
        font-size: $fontLittleSize;
        color: $grey;
        margin: 10px 0;
        }

        h2{
        font-size: $fontLittleSize;
        font-weight: 400;
        color: $blue;
        margin-bottom: 25px;

            span{
                color: $green;
            }
        }

        .description{
            color:  $grey;
            line-height: 2;

            i{
                color: $green;
                font-size: $fontMediumSize;
            }
        }

        .Ebook{
            margin-top: 35px;

            a{
            
                @include buttom;
            }
        }

    
    }

    .book{


        width:calc( 100% / 3);
        position: relative;
        cursor: pointer;

        img{
            width: 300px;
            
        }
            
        .book_name{
            @include flexContent;
            justify-content: center;
            color: $blue;
            font-weight: 600;
            margin-bottom: 10px
        }

        .book_price{
            @include flexContent;
            justify-content: center;
            color: $green;
            font-weight: 600;
        }

        .book_tools{
            display: none;
            position: absolute;
            top: 20%;
            right: 20%;
            z-index: 100;

            .tool{
                padding: 5px 7px;
                margin: 4px 0;
                border-radius: 50%;
                box-shadow: $shadow;

                a{
                    color: $grey;
                    
                    &:hover{
                        color: $black;
                    }
                }
            }

        }

        &:hover .book_tools{
            display: block;
        }

        
    }
   
}

/*  BRANDS */

#brands{
    @include container;
    @include flexContent;
    margin-top: 80px;

    img{
        width: 80px;
        filter: opacity(40%);;
            
    }
}


/* REAL STORIES */

#real_stories{
    @include container;
    @include flexContent;
    margin-top: 80px;
    width: $width;
    height: 400px;
    background-image: url("src/assets/images/1e237de1ae_Missy's Scribble Art1.jpg");
    object-fit: cover;
    position: relative;

    .story_description{
        @include flexContent;
        justify-content: center;
        width: $halfwidth;
        text-align: center;
        

        .description{
            width: 45%;

            h5{
                color: $green;
                font-size: $fontLittleSize;
                padding: 15px;
            }

            p{
                color: $black;
                font-weight: 600;
                padding: 15px;
            }

            img{
                width: 25%;
                border-radius: 50%;
            }

            .profession{
                color: $grey;
                padding: 10px;
                font-size: $fontLittleSize;
            }
        }

    }

    .story_img{
        width: $halfwidth;
        img{
            width: $width;
            height: 400px;
            object-fit: cover;
        }
    }

    .buttom_sliders{
        position: absolute;
        width: 75px;
        height: 75px;
        padding: 10px;
        border-radius: 50%;
        background-color: $white;
        box-shadow: $shadow;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        @include flexContent;
        justify-content: center;
        flex-direction: column;

        &:hover{
            width: 85px;
            height: 85px;
        }

        i{
            color: $grey;

            &:hover{
                color: $black;
                font-size: $fontMediumSize;
            }
        }

    }
    
}

/* ARTICLES */

#articles{
        @include container;
        margin-top: 80px;
        padding: $padding;

        h5{
            font-size: $fontLittleSize;
            color: $grey;
        }

        h2{
            font-weight: 400;
            padding: 20px 0;
            span{
                color: $green;
            }
        }

        .articles_container{
            @include flexContent;
            margin-top: 20px;

            .article{
                width: calc(100% / 5);
                padding: 8px;
                cursor: pointer;
                

                &:hover{
                    box-shadow:$shadow;
                }
                img{
                    width: $width;
                    object-fit: cover;
                    border-radius: 5px;

                }

                .date{
                    color: $fontLittleSize;
                    margin: 10px 0;
                    font-size: 12px;
                }

                h5{
                    color: $black;
                    margin: 10px 0;
                }

                p{
                    color: $grey;
                    font-size: $fontLittleSize;
                }
            }
        }

        a{
            margin-top: 50px;
            padding: 5px;
            color: $green;
            text-decoration: underline;
            @include flexContent;
            justify-content: center;
           

            &:hover{
                color: $blue;
            }
        }
    }


</style>