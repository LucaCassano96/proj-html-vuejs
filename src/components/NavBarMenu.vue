<script >


export default {
    name: "NavBarMenu",
    props:{
        links:Array,
    }
}

</script>

<template>

    <section id="nav_container">

        <div id="top" class="logo">
            <img src="src\assets\images\dark-logo.png" alt="">
        </div>

        <ul>
            <li  v-for='(link, index) in links' :key='index'>
                <a href="#">{{ link.navEl }} <i class="bi bi-caret-down"></i></a>
                
                    <ul class="hidden_menu">

                        <li v-for="submenus in link.NavMenu"><a href="#">{{ submenus}}</a></li>
                        

                    </ul> 
                
            </li>
        </ul>
    
        <div class="socials">

            <i class="bi bi-twitter"></i>
            <i class="bi bi-facebook"></i>
            <i class="bi bi-instagram"></i>
            <i class="bi bi-linkedin"></i>

        </div>

    </section>

</template>

<style lang="scss" scoped>
@use"../styles/partials/variables.scss" as*;
@use"../styles/general.scss" as*;

#nav_container{
    @include flexContent;
    width: $width;
    height: 80px;
    padding: $padding;

    .logo img{
        width: 150px;
    }

    ul{
        @include flexContent;
    li{
        position: relative;

        
        
         a{
            padding: 15px;
            color: $black;

            &:hover{
                color: $green;
                text-shadow: 0.2px 0.2px $green;
                text-decoration: underline;

            }
           
            
            i{
                font-size: $fontLittleSize;
                color: $black;
                
            }
        
        }
        .hidden_menu{
            width: 220px;
            background-color: $white;
            padding: $padding;
            position: absolute;
            display: none;
            z-index: 10;
        }
        &:hover .hidden_menu{
            display: block;
            box-shadow: $shadow;
            pointer-events: auto;
            border-bottom: 2px solid $green;

            li{
                padding: 10px 0;
            }
        }
        
    }
       
    }
    .socials i{
            padding: 10px;
            color: $black;
            
            &:hover{
                color: $blue;
                text-shadow: 0.2px 0.2px $blue;
                }
        }
}



</style>