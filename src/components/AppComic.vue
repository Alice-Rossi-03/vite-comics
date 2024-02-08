<script>
    export default{
        name: "AppComic",
        props:{
            img: String,
            title: String
        }
    }
</script>

<template>
   
    <div class="comic">
        <img :src="img" alt="">
        <div class="title">{{ title }}</div>
    </div>
 
    
</template>

<style scoped lang="scss">
    .container{
        

        .comic{
            width: calc((100% / 6) - 1em);

            img{
                width: 100%;
                // min-height: 235px;
                // min-height: 100%;
                aspect-ratio: 3/4;
            }

            .title{
                color: white;
                text-align: center;
            }
        }
    }
</style>