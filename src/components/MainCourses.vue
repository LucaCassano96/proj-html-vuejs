<script >


export default {
    name: "MainCourses",
    props:{
        course:Array,
    }
}

</script>

<template>


    <div class="card" v-for="(single_course,index) in course " :key='index'>
                
        <div>
            <img :src="single_course.img" alt="img course">
        </div>

        <div class="img_description">

            <div class="prize">
                ${{single_course.prize}}
            </div>

            <div class="description_course">
                {{ single_course.description }}
            </div>

            <div>
                <span><i class="bi bi-file-earmark-richtext"></i> {{single_course.lessons}}</span>
                <span><i class="bi bi-person"></i> {{single_course.students}}</span>
            </div>

        </div>    

    </div>

</template>

<style lang="scss" scoped>
@use"../styles/partials/variables.scss" as*;
@use"../styles/general.scss" as*;


.card{
    width: calc(100%/3 - 20px);
    margin-bottom: 20px;
    cursor: pointer;

    &:hover{
        box-shadow:$shadow;
        
    }

    img{
        width: $width;
        object-fit: cover;
    }
    .img_description{
        padding: $padding;
        .prize{
            color: $green;
            margin-bottom: 15px;
            font-weight: 700;
            font-size: $fontMediumSize;
        }

        .description_course{
            font-size: $fontMediumSize;
            font-weight: 700;
            color: $blue;
            margin-bottom: 15px;
        }

        span{
            margin-right: 20px;
        }

    }
    

}




</style>