<!-- parte logica (javascript) -->
<script>
export default {
    
}
</script>

<!-- parte grafica (html) -->
<template lang="">
    <header>
        <div class="row">
            <div class="col-logo">
                        

            </div>
            <div class="col-menu">
                        
            </div>
        </div>
    </header>
</template>

<!-- parte style (css/scss) -->
<style lang="scss" scoped> // inserito SASS allo style e inserito anche lo scope
    header{
        height: 100px;
        background-color: red;

        .row{
        max-width: 1170px;
        margin: 0 auto;
        display: flex;

            .col-logo{
                background-color: yellow;
                width: 50%;
                height: 100px;
            }
            .col-menu{
                background-color: rgb(0, 255, 217);
                width: 50%;
                height: 100px;
            }


        
        }
    }
    
    
</style>