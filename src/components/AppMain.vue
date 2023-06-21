<!-- parte logica (javascript) -->
<script>
export default {
    // boilerplate di Vue
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
                
            ]
        }
    }
    
}
</script>

<!-- parte grafica (html) -->
<template lang="">
    <main>
        <div class="container">
            <div class="row">
                <div class="col-100">
                    <div class="content">
                        <h2>--- Content goes here ---</h2>
                    </div>
                </div>
            </div>
        </div>
        <div class="container-menu">
            <div class="row-menu">
                <!-- ciclaggio delle voci di menu -->
                <div class="col-25" v-for="(item,index) in itemNewMenu">
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
        background-color: black;
        padding: 40px 0;




        .row{
            display: flex;
            max-width: 1170px;
            margin: 0 auto;
            display: flex;
            
        


            .col-100{
                color: white;
                display: flex;
                align-items: center;
                
                
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