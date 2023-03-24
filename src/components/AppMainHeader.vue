<script>
export default{
    data(){
      return{

        content: "--> Content goes here <--"
        



      }
  }
}


</script>

<template>
    <main class="main_container">

        <div class="centered">
    
            <h2>{{ content }}</h2>
            
        </div>

    </main>
</template>

<style lang="scss">

    .main_container{
        background-color: rgb(37, 37, 37);
        padding: 2rem 0;

        h2{
            color: white;
        }
    }

  
</style>