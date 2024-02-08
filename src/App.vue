<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooterOne from './components/AppFooterOne.vue'
import AppFooterTwo from './components/AppFooterTwo.vue'
import AppFooterThree from './components/AppFooterThree.vue'



export default{
    components: {
      AppHeader,
      AppMain,
      AppFooterOne,
      AppFooterTwo,
      AppFooterThree,
    }
  }
</script>

<template>
 
  <AppHeader/> 
  <AppMain/> 
  <AppFooterOne/> 
  <AppFooterTwo/> 
  <AppFooterThree/> 

</template>

<style lang="scss">
  @use './styles/general.scss'; 

</style>

  



