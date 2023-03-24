<script>

export default{
    data(){
      return{

        links:[
          "Character",
          "Comics",
          "Movies",
          "tv",
          "games",
          "collectibles",
          "videos",
          "fans",
          "news",
          "shop"
        ]



      }
  }
}

</script>

<template>
  <!-- header -->
    <header>

      <!-- navbar -->
      <nav class="centered">


        <!-- navleft -->
        <div class="nav_left">
          <img src="public/img/dc-logo.png" alt="">
        </div>

        <!-- navright -->
        <div class="nav_right">
          <ul>
            <li v-for="link in links">{{link}}</li>
          </ul>
        </div>

      </nav>
    </header>

</template>


<style lang="scss">

  nav{
    padding: 0 1rem;
    display: flex;
    align-items: center;
    justify-content: space-between;

  

    img{
      width: 60px;
    }

    
    ul{
      display: flex;

      li{
      padding: 25px 15px;
      text-transform: uppercase;

      color: gray;
      font-weight: bold;
      }


      li:hover{
        color: rgb(25, 116, 244);
        border-bottom: 2px solid  rgb(25, 116, 244);
      }

    }
  }



</style>