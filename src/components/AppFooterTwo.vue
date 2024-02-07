<template>
    <div class="footer">
        <div class="container">
            <div class="lists-container">
                <div>
                    <div>
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
                    <div></div>
                </div>
                <div></div>
                <div></div>
            </div>
            <figure>
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </figure>
        </div>
        
    </div>
</template>

<script>
    export default{
        name: 'AppFooterTwo'
    }
</script>

<style scoped>
    .footer{
        background-image: url(../assets/img/footer-bg.jpg);

        .container{
            width: 80%;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
        }
        
    }
</style>