<!-- parte logica (javascript) -->
<script>
export default {
    data(){
        // array per le liste 
        return{
            itemDcComics: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News'],
            itemShop: ['Shop DC', 'Shop DC Collectibles'],
            itemDC: ['Terms Of Use', 'Privacy policy (New)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscription', 'Talent Workshop', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us'],
            itemSites: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
        }
    }
    
}
</script>

<!-- parte grafica (html) -->
<template lang="">
    <footer>
        <div class="container-top-footer">
            <div class="row">
                <div class="col">
                    <!-- liste -->
                    <div class="first-list">
                        <ul>
                            <h2>DC COMICS</h2>
                            <!-- ciclaggio delle voci della prima lista -->
                            <li v-for="(item,index) in itemDcComics" :key="index">{{item}}</li>
                        </ul>
                        <ul id="sublist">
                            <h2>SHOP</h2>
                            <!-- ciclaggio delle voci della sottolista -->
                            <li v-for="(item,index) in itemShop" :key="index">{{item}}</li>
                           
                            
                        </ul>
                    </div>
                    <div class="second-list">
                        <ul>
                            <h2>DC </h2>
                            <!-- ciclaggio delle voci della seconda lista -->
                            <li v-for="(item,index) in itemDC" :key="index">{{item}}</li>
                        </ul>

                    </div>
                    <div class="third-list">
                        <ul>
                            <h2>SITES</h2>
                            <!-- ciclaggio delle voci della terza lista -->
                            <li v-for="(item,index) in itemSites" :key="index">{{item}}</li>
                        </ul>

                    </div>

                </div>
                
            </div>
        </div>
        <div class="container-end-footer">
            <div class="row">
                <div class="col-button">
                    <button>SIGN-UP NOW</button>

                </div>
                <div class="col-social">
                    <h3>FOLLOW US</h3>
                    <!-- icone social -->
                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt="">
                    
                </div>

            </div>
        </div>

    </footer>
</template>

<!-- parte style (css/scss) -->
<style lang="scss" scoped> // inserito SASS allo style e inserito anche lo scope
    .container-top-footer{
        background-image: url('../assets/img/footer-bg.jpg');
        


        .row{
            display: flex;
            max-width: 1170px;
            margin: 0 auto;
            display: flex;
            background-image: url('../assets/img/dc-logo-bg.png');
            background-size: 500px;
            background-repeat: no-repeat;
            background-position: right;
            padding: 40px 0;
            padding-bottom: 60px;



            .col{
                display: flex;

                ul{
                    list-style-type: none;
                    padding-right: 40px;
                    color: rgba(243, 243, 243, 0.531);

                    li{
                        &:hover{
                            color: white;
                        }
                    }

                    h2{
                        padding-bottom: 10px;
                        color: white;
                    }
                }
                #sublist{
                    padding-top: 10px;
                }
            }
        }    
        

    }

    .container-end-footer{
        background-color: rgb(62, 62, 62);
        padding: 20px 0;


        .row{
            display: flex;
            max-width: 1170px;
            margin: 0 auto;
            display: flex;


            .col-button{
                width: 50%;
                display: flex;
               


                button{
                    background-color: transparent;
                    padding: 15px;
                    border-color: rgb(5, 136, 237);
                    color: white;
                    font-weight: 800;
                }
                
            }

            .col-social{
                width: 50%;
                display: flex;
                justify-content: end;


                
                h3{
                    color: rgb(38, 143, 234);
                    padding-top: 10px;
                    padding-right: 40px;
                }
                img{
                    margin-right: 10px;
                    height: 30px;
                    margin-top: 5px;

                    &:hover{
                        background-color: white;
                    }
                }
            }

        }
    }
    
</style>