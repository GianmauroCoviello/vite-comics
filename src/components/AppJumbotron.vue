<!-- componente logica (javascript) -->
<script>
export default {
    
}
</script>

<!-- componente grafica (html) -->
<template lang="">
    <!-- container che conterra il jumbotron -->
    <div class="container-jumbotron">
        <div class="row">
            <!-- button che avrà la proprietà position per posizionarsi -->
            <button><h2>CURRENT SERIES</h2></button>
        </div>
        
    </div>
</template>

<!-- componente style (css/scss) -->
<style lang="scss" scoped>
    .container-jumbotron{
        background-image: url('../assets/img/jumbotron.jpg');
        background-size: cover;
        padding: 160px 0;
        position: relative;

        .row{
            max-width: 1170px;
            margin: 0 auto;
            

            button{
            padding: 10px 20px;
            background-color: rgb(46, 116, 255);
            border: none;
            color: white;
            font-weight: 900;
            position: absolute;
            top: 298px;
            
            
            }
        }
        
    }
    
</style>