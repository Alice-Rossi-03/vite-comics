<template>
    <footer class="bg-dark">
        <div class="container">
            <div class="button">
                <a href="#">SIGN-UP NOW</a>
            </div>
            <div class="icons">
                <div class="blue">FOLLOW US</div>
                <figure v-for="(element, index) in socialList" :key="index">
                    <img :src="element.img" alt="">
                </figure>
            </div>
        </div>
    </footer>
</template>

<script>
    export default{
        name: 'AppFooterThree',
        data(){
            return{
                socialList: [
                    {
                        name: "Facebook",
                        img: "src/assets/img/footer-facebook.png"
                    },
                    {
                        name: "Twitter",
                        img: "src/assets/img/footer-twitter.png"
                    },
                    {
                        name: "YouTube",
                        img: "src/assets/img/footer-youtube.png"
                    },
                    {
                        name: "Pinterest",
                        img: "src/assets/img/footer-pinterest.png"
                    },
                    {
                        name: "Maps",
                        img: "src/assets/img/footer-periscope.png"
                    },
                ]
            }
        }
    }
</script>

<style scoped>
    .bg-dark{
        background-color: #303030;

        .container{
            width: 80%; 
            margin: 0 auto;
            padding-block: 2em;
            display: flex;
            align-items: center;
            justify-content: space-between;

            .button{
                a{
                    color: white;
                    text-decoration: none;
                    padding: 0.5em;
                    border: 0.2em solid #2282F9;

                    &:hover{
                        opacity: 0.8;
                    }
                }
            }

            .icons{
                display: flex;
                gap: 1em;
                align-items: center;

                .blue{
                    color:#2282F9; 
                    font-size: 1.5em;
                }
            }
        }
    }
</style>