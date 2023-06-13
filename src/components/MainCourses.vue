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
        box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
        
    }

    img{
        width: 100%;
        object-fit: cover;
    }
    .img_description{
        padding: 20px;
        .prize{
            color: $green;
            margin-bottom: 15px;
            font-weight: 700;
            font-size: 18px;
        }

        .description_course{
            font-size: 18px;
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