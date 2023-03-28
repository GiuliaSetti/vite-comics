<script>
    // navbar
    import AppNavbar from './components/AppNavbar.vue';
    // main
    import AppMain from './components/AppMain.vue';
    // buy items
    import AppBuy from './components/AppBuy.vue';
    // footerup
    import AppFooterUp from './components/AppFooterUp.vue';


        export default {
          data() {
            return {
              
            }
          },
          components: {
            AppNavbar,
            AppMain,
            AppBuy,
            AppFooterUp,
          }
    }

</script>

<template>

  <!-- navbar -->
  <AppNavbar></AppNavbar>

  <!-- main -->
  <AppMain></AppMain>

  <!-- buy_items -->
  <AppBuy></AppBuy>

  <!-- footerUp -->
  <AppFooterUp></AppFooterUp>




</template>

<style lang="scss" scoped>
</style>