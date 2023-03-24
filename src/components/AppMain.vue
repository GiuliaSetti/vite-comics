<script>
export default{
    data(){
      return{

        main:[
            {
                image: "../public/img/buy-comics-digital-comics.png",
                link: "digital comics"
            },
            {
                image: "../public/img/buy-comics-merchandise.png",
                link: "dc merchandise"
            },
            {
                image: "../public/img/buy-comics-subscriptions.png",
                link: "subscription"
            },
            {
                image: "../public/img/buy-comics-shop-locator.png",
                link: "comic shop locator"
            },
            {
                image: "../public/img/buy-dc-power-visa.svg",
                link: "dc power visa"
            }
        ]
        



      }
  }
}

</script>

<template>
    <div class="main_container_blue">
        <ul>
            <li v-for="element in main"><img :src="element.image" alt="">{{element.link}}</li>
          
        </ul>
        
    </div>
</template>

<style lang="scss">

    .main_container_blue{
        background-color: rgb(25, 116, 244);


        ul{
            color: white;
            display: flex;
            padding: 4rem 10rem;

            justify-content: space-around;

        li{
            display: flex;
            align-items: center;
            gap: 10px;

            img{
                width: 50px;
                display: block;
            }

            text-transform: uppercase;

        }
    }
    }

  


</style>