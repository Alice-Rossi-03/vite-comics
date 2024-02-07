<template>
    <div class="footer">
        <div class="container">
            <div class="container-flex">
                <div v-for="(element, index) in footerList" :key="index" class="container-mini-flex">
                    <figure style="min-height: 2em; min-width: 2em;">
                        <img :src="element.img" alt="img">
                    </figure>
                    <div>{{ element.name }}</div>

                </div>
            </div>
        </div>
    </div>
    
</template>

<script>
    export default{
        name: 'AppFooterOne',
        data(){
            return{
                footerList:[
                    {
                        name: "DIGITAL COMICS",
                        img: "src/assets/img/buy-comics-digital-comics.png"
                    },
                    {
                        name: "DC MERCHANDISE",
                        img: "src/assets/img/buy-comics-merchandise.png"
                    },
                    {
                        name: "SUBSCRIPTION",
                        img: "src/assets/img/buy-comics-subscriptions.png"
                    },
                    {
                        name: "COMIC SHOP LOCATOR",
                        img: "src/assets/img/buy-comics-shop-locato.png"
                    },
                    {
                        name: "DC POWER VISA",
                        img: "src/assets/img/buy-dc-power-visa.svg"
                    }
                    
                ]
            }
        }
    }
</script>

<style scoped>

    .footer{
        background-color: #207CEC;

        .container{
            width: 80%;
            padding-block: 3em;
            color: white;
            margin: 0 auto;
            font-size: 1.2em;

            .container-flex{

                display: flex;
                gap: 2em;
                justify-content: center;

                .container-mini-flex{
                    display: flex;
                    gap: 0.5em;
                    align-items: center;

                    figure{
                        width: 3em;
                        height: 3em;

                        img{
                            max-width: 100%;
                            height: 100%;
                            /* display: block; */
                        }
                    }
                }
                
            }

            
        }

            
        
    }

</style>