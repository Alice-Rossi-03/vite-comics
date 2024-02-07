<template>
    <header>
        <div class="bg-white">
            <div class="container">
                <figure>
                    <img src="../assets/img/dc-logo.png" alt="logo">
                </figure>

                <ul>
                    <li v-for="(element, index) in navBarList" :key="index">
                        <a href="element.path">
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
                        current: true
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



</style>