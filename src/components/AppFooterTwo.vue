<template>
    <div class="footer">
        <div class="container">
            <div class="lists-container">
                <div class="list-con">
                    <div class="list">
                        <h3>DC COMICS</h3>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                    </div>
                    <div class="list">
                        <h3>SHOP</h3>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li> 
                            
                        </ul>
                    </div>
                </div>
                <div class="list-con">
                    <div class="list">
                        <h3>DC</h3>
                        <ul>
                            <li>Terms Of Use</li>
                            <li>Privacy Policy (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent workshop</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>
                </div>
                <div class="list-con">
                    <div class="list">
                        <h3>SITES</h3>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                            
                        </ul>
                    </div>
                </div>
            </div>
            <figure>
                <!-- <img src="../assets/img/dc-logo-bg.png" alt=""> -->
            </figure>
        </div>
        
    </div>
</template>

<script>
    export default{
        name: 'AppFooterTwo'
    }
</script>

<style scoped lang="scss">
@use '../styles/partials/_variables.scss' as *; 


    .footer{
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;

        .container{
            width: 80%;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;

            figure{
                background-image: url(../assets/img/dc-logo-bg.png);
                width: 1000px;
                /* background-size: contain; */
                background-position: right;
                background-repeat: no-repeat;
            }

            .lists-container{
                padding-top: 3em;
                display: flex;
                gap: 3.5em;

                .list-con{

                    .list{
                        margin-bottom: 2em;

                        h3{
                            color: $white;
                            margin-bottom: 0.5em;
                        }

                        ul{
                            li{
                                list-style-type: none;
                                color: $gray; 
                                margin-bottom: 0.2em;
                                font-family: 'PT Sans Narrow', sans-serif;
                                font-weight: 400;
                            }
                        }
                    }
                }
            }
        }
        
    }
</style>