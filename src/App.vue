<script>
    // navbar
    import AppNavbar from './components/AppNavbar.vue';
    // main
    import AppMain from './components/AppMain.vue';

        export default {
          data() {
            return {
              
            }
          },
          components: {
            AppNavbar,
            AppMain,
          }
    }

</script>

<template>

  <!-- navbar -->
  <AppNavbar></AppNavbar>

  <!-- main -->
  <AppMain></AppMain>




</template>

<style lang="scss" scoped>
</style>