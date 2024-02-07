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

<style scoped lang="scss">
@use '../styles/partials/_variables.scss' as *; 

    .bg-white{
        background-color: $white;

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
                    font-size: 0.9em;

                    a{
                        text-decoration: none;
                        color: $black;
                        height: 100% ;
                        padding-bottom: 3.3em;

                        &:hover{
                            color: $blue;
                            border-bottom: 0.5em solid $blue;
                        }
                    }   

                    .active{
                            color: $blue;
                            border-bottom: 0.5em solid $blue;
                        }
                }

            }
        }


    }

</style>