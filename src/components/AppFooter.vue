<script>
    export default{
        data(){
        return{

            imagesList:[
                "../public/img/footer-facebook.png",
                "../public/img/footer-periscope.png",
                "../public/img/footer-pinterest.png",
                "../public/img/footer-twitter.png",
                "../public/img/footer-youtube.png"
            ]

        }
     },
    }
</script>

<template>
    <div class="footer_container">

        <div class="footer_down centered">
            <div class="footer_left">
                <button>SIGN-UP NOW</button>

            </div>

            <div class="footer_right">
                <div>FOLLOW US</div>

                <ul>
                    <li v-for="element in imagesList"><img :src="element" alt="immagine"></li>
                </ul>

            </div>

        </div>

    </div>
</template>

<style lang="scss">

    .footer_container{
        padding: 1rem;
        background-color: rgb(74, 74, 74);

        .footer_down{
            display: flex;
            justify-content: space-between;

            
            button{
                padding: 10px 20px;
                background-color: transparent;
                border: 2px solid rgb(25, 116, 244);
                color: white;
                font-weight: bold;
        
            }

            .footer_right{
                display: flex;
                align-items: center;
                gap: 20px;

                div{
                    color: rgb(25, 116, 244);
                    font-weight: bold;
                }

                ul{
                    display: flex;
                    gap: 10px;
                }
            }

        }

    }

  
</style>