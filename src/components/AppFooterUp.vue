<script>
    export default{
        name:'AppFooterUp',
        data(){
        return{
            image: '../public/img/dc-logo-bg.png',
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
        <div id="footer" class="centered">
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

            <div class="background_logo">
                <img :src="image" alt="logo">
            </div>

        </div>
    </div>

</template>

<style lang="scss" scoped>


    .footer_up_container{
            background-image: url(../public/img/footer-bg.jpg);
            background-size: cover;

            overflow-y: hidden;


            #footer{
                padding: 2rem;
                display: flex;
                gap: 20px;

                position: relative;

                .background_logo{

                    position: absolute;

                    top: -100px;
                    right: 20px;

                }
                

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
                color: #7b7b7b;
            }
    }


</style>