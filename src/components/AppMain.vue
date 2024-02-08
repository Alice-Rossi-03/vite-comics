<script>
    import AppJumbotron from '../components/inner-main-components/AppJumbotron.vue'
    import AppComics from '../components/inner-main-components/AppComics.vue'
    
    export default{
        name: 'AppMain',
        components: {
            AppJumbotron,
            AppComics
        }
    }
</script>

<template>
    <main>
        <AppJumbotron/>
        <AppComics/>
    </main>
    
</template>

<style scoped lang="scss">
@use '../styles/partials/_variables.scss' as *; 

    main{
        background-color: $black;
    }

</style>