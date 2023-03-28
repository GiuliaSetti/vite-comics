<script>

    // singolo fumetto
    import ComicItem from './ComicItem.vue'

    export default {
    name: "AppMain",
    data() {
        return {
            activePageTitle: 'current series',
            comics: [
                {
                    thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    price: "$19.99",
                    series: "Action Comics",
                    type: "comic book"
                },
                {
                    thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    price: "$3.99",
                    series: "American Vampire 1976",
                    type: "comic book"
                },
                {
                    thumb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560,c_limit/Aquaman-16.jpg",
                    price: "$16.99",
                    series: "Aquaman",
                    type: "graphic novel"
                },
                {
                    thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    price: "$2.99",
                    series: "Batgirl",
                    type: "comic book"
                },
                {
                    thumb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    price: "$3.99",
                    series: "Batman",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    price: "$2.99",
                    series: "Batman Beyond",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    price: "$4.99",
                    series: "Batman/Superman Annual",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel"
                }
            ],
           
          };
          
    },

    components:{
        ComicItem,
    }

}
  
</script>


<template>

    <main class="container">

       
        <div id="jumbotron">

        </div>

        <div id="main_content" class="centered">
            <!-- titolo -->
            <h4>{{ activePageTitle }}</h4>

            <div id="comics">

                <!-- singolo fumetto -->
                <ComicItem v-for="comic in comics"  :cover="comic.thumb" :title="comic.series"></ComicItem>

            </div>

            <div class="button">
                <button>Load More</button>
            </div>

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

            #comics{
                padding: 0 1rem;
                padding-top: 4rem;
                display: flex;
                flex-flow: row wrap;

                gap: 40px 20px;
            }

            .button {

                text-align: center;
                padding: 2rem;




                button{
                    padding: 10px 45px;
                    background-color: $mainColor;
                    border: none;
                    color: white;
                    text-transform: uppercase;
                    font-weight: bold;

                    cursor: pointer;

         
                }
            }
          


            
        }

        
    }




</style>