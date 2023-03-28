<script>
    // navbar
    import AppNavbar from './components/AppNavbar.vue';
    // main
    import AppMain from './components/AppMain.vue';
    // buy items
    import AppBuy from './components/AppBuy.vue';

        export default {
          data() {
            return {
              
            }
          },
          components: {
            AppNavbar,
            AppMain,
            AppBuy,
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




</template>

<style lang="scss" scoped>
</style>