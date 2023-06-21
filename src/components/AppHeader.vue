<!-- parte logica (javascript) -->
<script>
export default {
    data(){
        return{
            // array di oggetti per le voci di menu
            itemMenu: [
                {
                    nome: 'CHARACTERS',
                    active : false,
                    link: '#'
                },
                {
                    nome: 'COMICS',
                    active : true,
                    link: '#'
                },
                {
                    nome: 'MOVIES',
                    active : false,
                    link: '#'
                },
                {
                    nome: 'TV',
                    active : false,
                    link: '#'
                },
                {
                    nome: 'COLLECTIBLES',
                    active : false,
                    link: '#'
                },
                {
                    nome: 'VIDEOS',
                    active : false,
                    link: '#'
                },
                {
                    nome: 'FANS',
                    active : false,
                    link: '#'
                },
                {
                    nome: 'NEWS',
                    active : false,
                    link: '#'
                },
                {
                    nome: 'SHOP',
                    active : false,
                    link: '#'
                    
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
                    <!-- ciclaggio dei nomi delle voci di menu -->
                    <li v-for="(item,index) in itemMenu" :class="item.active ? 'active':''" :key="index" >
                        <a  :href="item.link">{{item.nome}}</a>
                    </li>
                </ul>
                        
            </div>
        </div>
    </header>
</template>

<!-- parte style (css/scss) -->
<style lang="scss" scoped> // inserito SASS allo style e inserito anche lo scope
    .active{
        border-bottom: 4px solid blue;
    }
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
                        // border-bottom: 4px solid rgb(255, 255, 255);
                        cursor: pointer;
                       
                        


                        a{
                            text-decoration: none;
                            color: rgba(0, 0, 0, 0.92);

                            
                        }

                        
                        &:hover a{
                            color: blue;
                        }

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