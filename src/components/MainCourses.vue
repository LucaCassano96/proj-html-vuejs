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
                {{single_course.prize}}
            </div>
            <div class="description_course">
                {{ single_course.description }}
            </div>

            <div>
                <span>{{single_course.lessons}}</span>
                <span>{{single_course.students}}</span>
            </div>

        </div>    

    </div>

</template>

<style lang="scss" scoped>
@use"../styles/partials/variables.scss" as*;
@use"../styles/general.scss" as*;


.card{
    width: calc(100%/3 - 20px);
    border:1px solid #000 ;
    margin-bottom: 20px;

    img{
        width: 100%;
        object-fit: cover;
    }
}




</style>