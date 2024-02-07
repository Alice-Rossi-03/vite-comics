<template>
    <header>
        <div class="bg-white">
            <div class="container">
                <figure>
                    <img src="../assets/img/dc-logo.png" alt="logo">
                </figure>

                <ul>
                    <li v-for="(element, index) in navBarList" :key="index">
                        <a href="element.path" :class="(element.current) ? 'active' : '' ">
                            {{ element.name }}
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
    
</template>

<script>

    export default{
        name: 'AppHeader',
        data(){
            return{
                navBarList: [
                    {
                        name: 'CHARACTERS' ,
                        path: '#', 
                        current: true
                    }, 
                    {
                        name: 'COMICS' ,
                        path: '#', 
                        current: false
                    }, 
                    {
                        name: 'MOVIES' ,
                        path: '#', 
                        current: false
                    }, 
                    {
                        name: 'TV' ,
                        path: '#', 
                        current: false
                    }, 
                    {
                        name: 'GAMES' ,
                        path: '#', 
                        current: false
                    }, 
                    {
                        name: 'COLLECTIBLES' ,
                        path: '#', 
                        current: false
                    }, 
                    {
                        name: 'VIDEOS' ,
                        path: '#', 
                        current: false
                    }, 
                    {
                        name: 'FANS' ,
                        current: false
                    }, 
                    {
                        name: 'NEWS' ,
                        path: '#', 
                        current: false
                    }, 
                    {
                        name: 'SHOP' ,
                        path: '#', 
                        current: false
                    }, 
                ]
            }
        }
    }

</script>

<style scoped>

    .bg-white{
        background-color: white;

        .container{
            width: 80%;
            margin: 0 auto;
            display: flex;
            align-items: center;
            justify-content: space-between;
            height: 8em;

            figure{
                align-self: center;
            }

            ul{
                display: flex;
                gap: 1em;

                li{
                    list-style-type: none;
                    font-size: 0.7em;

                    a{
                        text-decoration: none;
                        color: black;
                        height: 100% ;
                        padding-bottom: 4.6em;

                        &:hover{
                            color: #207CEC;
                            border-bottom: 0.4em solid #207CEC  ;
                        }
                    }   

                    .active{
                            color: #207CEC;
                            border-bottom: 0.4em solid #207CEC  ;
                        }
                }

            }
        }


    }

</style>