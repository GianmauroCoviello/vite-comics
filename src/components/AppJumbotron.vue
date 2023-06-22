<!-- componente logica (javascript) -->
<script>
export default {
    
}
</script>

<!-- componente grafica (html) -->
<template lang="">
    <!-- container che conterra il jumbotron -->
    <div class="container-jumbotron">
        <button><h2>CURRENT SERIES</h2></button>
    </div>
</template>

<!-- componente style (css/scss) -->
<style lang="scss" scoped>
    .container-jumbotron{
        background-image: url('../assets/img/jumbotron.jpg');
        background-size: cover;
        padding: 160px 0;
        position: relative;


        button{
            padding: 10px 20px;
            background-color: rgb(46, 116, 255);
            border: none;
            color: white;
            font-weight: 900;
            position: absolute;
            top: 298px;
            left: 80px;
            
        }
    }
    
</style>