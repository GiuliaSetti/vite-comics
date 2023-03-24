<script>

export default{
    data(){
      return{

        footerRightColumn:[
            {
                title: "dc comics",
                links:[
                   "Character",
                    "Comics",
                    "Movies",
                    "TV",
                    "Games",
                    "Videos",
                    "News",
                ]
               
            },

            {
                title:"shop",
                links:[
                    "Shop Dc",
                    "Shop DC Collectibles"
                ]
            },

      
           
        ],

        footerLeftColumn:[
            {
                title:"dc",
                links:[
                    "Terms Of Use",
                    "Privacy police(New)",
                    "Ad Choices",
                    "Advertising",
                    "Jobs",
                    "Subscriptions",
                    "Talent Workshops",
                    "CPSC Certificates",
                    "Ratings",
                    "Shop Help",
                    "Contact Us"
                ]
            },

            {
                title:"sites",
                links:[
                    "DC",
                    "MAD Magazine",
                    "DC Kids",
                    "DC Universe",
                    "DC Visa"
                ]
            },


        ]

      }
  },
}
</script>


<template>
    <div class="footer_up_container">
        <div class="footer centered">
            <div class="right_list">

                <ul v-for="element in footerRightColumn">
                    <div>{{element.title}}</div>
                    <li v-for="link in element.links">{{link}}</li>
                </ul>

            </div>
    

            <ul v-for="element in footerLeftColumn">
                <div>{{element.title}}</div>
                <li v-for="link in element.links">{{link}}</li>
            </ul>

        </div>
    </div>
</template>

<style lang="scss">

    .footer_up_container{
        background-image: url(../public/img/footer-bg.jpg);
        background-size: cover;



        .footer{

            padding: 2rem;
            display: flex;
            gap: 20px;

            ul{
                div{
                    font-weight: bold;
                    text-transform: uppercase;
                    font-size: 20px;
                    color: white;
                    padding: 0.5rem 0;
                }
            }

            .right_list{
                display: flex;
                flex-direction: column;
                gap: 10px;
            }

            color: rgb(109, 109, 109);
        }
    }

</style>