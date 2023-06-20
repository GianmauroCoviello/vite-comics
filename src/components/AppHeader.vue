<!-- parte logica (javascript) -->
<script>
export default {
    data(){
        return{
            itemMenu: [
                {
                    nome: 'CHARACTERS'
                },
                {
                    nome: 'COMICS'
                },
                {
                    nome: 'MOVIES'
                },
                {
                    nome: 'TV'
                },
                {
                    nome: 'COLLECTIBLES'
                },
                {
                    nome: 'VIDEOS'
                },
                {
                    nome: 'FANS'
                },
                {
                    nome: 'NEWS'
                },
                {
                    nome: 'SHOP'
                },
            ]
        }
    }
    
    
}
</script>

<!-- parte grafica (html) -->
<template lang="">
    <header>
        <div class="row">
            <div class="col-logo">
                <img src="../assets/img/dc-logo.png" alt="">
                        

            </div>
            <div class="col-menu">
                <ul>
                    <li v-for="(item,index) in itemMenu">{{item.nome}}</li>
                </ul>
                        
            </div>
        </div>
    </header>
</template>

<!-- parte style (css/scss) -->
<style lang="scss" scoped> // inserito SASS allo style e inserito anche lo scope
    header{
        
        

        .row{
        max-width: 1170px;
        margin: 0 auto;
        display: flex;

            .col-logo{
                width: 40%;

                img{
                    width: 80px;
                    padding: 15px 0;
                }
                
            }
            .col-menu{
                width: 70%;
                display: flex;
                align-items: center;
                justify-content: flex-end;
                


                ul{
                    list-style-type: none;
                    display: flex;
                    height: 100%;
                    
                    
                    
                    li{
                        margin-right: 20px;
                        display: flex;
                        align-items: center;
                       

                        
                        

                        &:hover{
                            border-bottom: 4px solid blue;
                            cursor: pointer;
                        }
                        
                    }
                }
            }


        
        }
    }
    
    
</style>