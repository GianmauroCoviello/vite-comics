<!-- parte logica (javascript) -->
<script>
import AppListCards from './AppListCards.vue';
export default {
    // boilerplate di Vue
    components:{
        AppListCards
    },
    data(){
        return{
            // array di oggetti per le caratteristiche delle voci del menu
            itemNewMenu: [
                {   
                    src_image: '../src/assets/img/buy-comics-digital-comics.png',
                    nome: 'DIGITAL COMICS',
                },
                {
                    src_image: '../src/assets/img/buy-comics-merchandise.png',
                    nome: 'DC MERCHANDISE',
                },
                {
                    src_image: '../src/assets/img/buy-comics-subscriptions.png',
                    nome: 'SUBSCRIPTION',
                },
                {
                    src_image: '../src/assets/img/buy-comics-shop-locator.png',
                    nome: 'COMIC SHOP LOCATOR',
                },
                {
                    src_image: '../src/assets/img/buy-dc-power-visa.svg',
                    nome: 'DC POWER VISA',
                },
                
            ],
            cards : [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel",
                },
            ]
        }
    }
    
}
</script>

<!-- parte grafica (html) -->
<template lang="" >
    <main>
        <div class="container">
            <div class="row">
                <AppListCards v-for="(card,index) in cards" :image="card.thumb" />
            </div>
            
        </div>
        
        
        
        <div class="container-menu">
            <div class="row-menu">
                <!-- ciclaggio delle voci di menu -->
                <div class="col-25" v-for="(item,index) in itemNewMenu" :key="index">
                    <img :src="item.src_image" alt=""> <!--contiene l'src dell' immagine--> 
                    <p>{{item.nome}}</p> <!--contiene il nome dell' immagine--> 
                    
                </div>
            </div>
        </div>
    </main>
</template>

<!-- parte style (css/scss) -->
<style lang="scss" scoped> // inserito SASS allo style e inserito anche lo scope
    .container{
        background-color: rgb(29, 27, 27);
        padding: 30px 0;

        .row{
            display: flex;
            max-width: 1170px;
            margin: 0 auto;
            flex-wrap: wrap;


            .card{
                border: 2px solid white;
                width: calc(100%/6 - 20px);
                margin: 10px;
                color: white;
                

                
            }

        }
    }

    .container-menu{
        background-color: rgb(58, 101, 242);
        



        .row-menu{
            display: flex;
            max-width: 1170px;
            margin: 0 auto;
            display: flex;
            

            .col-25{
                width: calc(100%/5);
                color: white;
                display: flex;
                padding-left: 10px;
                padding: 40px 0;
                justify-content: center;

                &:hover{
                    background-color: rgb(14, 34, 102);
                    
                }


                img{
                    height: 60px;
                    
                
                }
                p{
                    align-self: center;
                    padding:0 10px ;
                    font-size: 12px;
                }
                
            }
        }
    
    }
</style>