<script>
    export default{
        name:'AppBuy',
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

    <div id="buy_container">
        <ul class="centered">
            <li v-for="element in main"><img :src="element.image" alt="">{{element.link}}</li>
          
        </ul>
        
    </div>

</template>

<style lang="scss">

@use "../scss/variables" as *;

    #buy_container{
            background-color: $mainColor;
            ul{
                padding: 2rem;
                color: white;
                display: flex;
                justify-content: space-between;
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