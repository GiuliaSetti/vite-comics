83 lines (60 sloc)  1.69 KB

<script>
    export default{
        name:'AppFooter',
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

<style lang="scss" scoped>


@use "../scss/variables" as *;
    .footer_container{
        padding: 1rem;
        background-color: #303030;
        .footer_down{
            display: flex;
            justify-content: space-between;
            
            button{
                padding: 10px 20px;
                background-color: transparent;
                border: 2px solid $mainColor;
                color: white;
                font-weight: bold;
        
            }
            .footer_right{
                display: flex;
                align-items: center;
                gap: 20px;
                div{
                    color: $mainColor;
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