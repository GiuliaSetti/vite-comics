<script>
    export default {
    name: "AppNav",
        data() {
            return {
                links: [
                    'characters',
                    'comics',
                    'movies',    
                    'tv',
                    'games',
                    'collectibles',
                    'videos',
                    'fans',
                    'news',
                    'shop',
                ],

                currentIndex: 1,
            }
        },

        methods: {
            indexUp(upIndex) {
                
                this.currentIndex = upIndex;  
                console.log(upIndex)
            }
            
        }
    }
</script>


<template>

    <nav >

        <div class="nav_content centered">

            <div id="nav_left">

                <div id="logo_container">

                    <img src="/img/dc-logo.png" alt="logo">

                </div>

            </div>

            <div id="nav_right">

                <ul>
                    <li v-for="(link, index) in links" class="link" :class="currentIndex == index ? 'active' : ''" @click="indexUp(index)"><a href="#">{{ link }}</a></li>
                </ul>

            </div>

        </div>
       

    </nav>


</template>


<style lang="scss" scoped>

    @use "../scss/variables" as *;

    nav{
        
        position: fixed;
        background-color: white;

        width: 100vw;
        height: 85px;
       

        .nav_content{

            display: flex;
            justify-content: space-between;
            align-items: center;
            
        #nav_left{
            #logo_container{
                width: 70px;

                img{
                    width: 100%;
                }
            }

        }

        #nav_right{
            
            ul {
                display: flex;
                gap: 20px;
                color: #464646;

                li{
                    position: relative;
                    padding: 2rem 0;
                    
                    a {
                        color: inherit;
                        text-decoration: none;
                        text-transform: uppercase;
                        font-weight: bold;
                    }
                        &.active {
                        color: $mainColor;
                        
                            &::before {
                                content: '';

                                width: 100%;
                                height: 3px;
                            
                                background-color: $mainColor;

                                position: absolute;
                                bottom: 0;
                            }
                        }
                    
                }
            }

        }


        }
        
      





    }


</style>