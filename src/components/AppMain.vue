<template>
    <main>
        <div class="container">
            <div>
                -- Content -- 
            </div>
        </div>
    </main>
    
</template>

<script>
    export default{
        name: 'AppMain'
    }
</script>

<style scoped lang="scss">
@use '../styles/partials/_variables.scss' as *; 

    main{
        background-color: $black;

        .container{
            width: 80%;
            padding-block: 3em;
            color: white;
            margin: 0 auto;
            font-size: 1.5em;
        }

    }

</style>