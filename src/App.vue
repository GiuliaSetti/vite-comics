<script>

  import AppNavbar from './components/AppNavbar.vue'
  import AppMainHeader from './components/AppMainHeader.vue'
  import AppMain from './components/AppMain.vue'
  import AppFooterUp from './components/AppFooterUp.vue'
  import AppFooter from './components/AppFooter.vue'

  export default{
    data(){
      return{

      }
  },


  components:{
    AppNavbar,
    AppMainHeader,
    AppMain,
    AppFooterUp,
    AppFooter
  }
}

</script>


<template>

  <div>
    <AppNavbar></AppNavbar>
  </div>

 

  <div>
    <AppMainHeader></AppMainHeader>
    <AppMain></AppMain>
  </div>

  <div>
    <AppFooterUp></AppFooterUp>
    <AppFooter></AppFooter>
  </div>



</template>

<style lang="scss">

 


</style>