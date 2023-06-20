<!-- parte logica (javascript) -->
<script>
export default {
    
}
</script>

<!-- parte grafica (html) -->
<template lang="">
    <main>
        <div class="container">
            <div class="row">
                <div class="col-100">
                    <div class="content">
                        <h2>--Content goes here--  </h2>
                    </div>
                </div>
            </div>
        </div>
        <div class="container-menu">
            <div class="row-menu">
                <div class="col-25">
                    1
                    
                </div>
                <div class="col-25">
                    2
                    
                </div>
                <div class="col-25">
                    3
                    
                </div>
                <div class="col-25">
                    4
                    
                </div>
                <div class="col-25">
                    5
                    
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
        height: 100px;



        .row-menu{
            display: flex;
            max-width: 1170px;
            margin: 0 auto;
            display: flex;

            .col-25{
                width: calc(100%/5);

            }
        }
    
    }
</style>