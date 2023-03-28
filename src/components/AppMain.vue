<script>

    export default {
    name: "AppMain",
    data() {
        return {
            activePageTitle: 'current series',
           
          };
          
    },

}
  
</script>


<template>

    <main class="container">

       
        <div id="jumbotron">

        </div>

        <div id="main_content" class="centered">
            <!-- titolo -->
            <h4>{{ activePageTitle }}</h4>
        </div>

    </main>

    


</template>


<style lang="scss" scoped>

@use "../scss/variables" as *;

    .container{
        background-color: #1C1C1C;
        padding-top: 85px;

        #jumbotron{

            height: 300px;
            background-image: url(../public/img/jumbotron.jpg);
            background-size: cover;
        }

        #main_content{

            position: relative;

            h4{
                width: 180px;
                padding: 10px 5px;

                text-align: center;
                text-transform: uppercase;

                background-color: $mainColor;
                color: white;

                position: absolute;
                top: -20px;
            }


            
        }

        
    }




</style>