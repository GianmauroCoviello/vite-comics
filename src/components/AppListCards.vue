<!-- parte logica (javascript) -->
<script>

export default {
    // inseriamo il promps con i nomi delle variabili
    props:{
        // variabili che rappresentano le singole informazioni dell'array di oggetti indicandone il tipo di dato che viene inserito (string,num ecc..)
        image: String, 
        title: String
    }
    
    
}
</script>

<!-- parte grafica (html) -->
<template lang="">
    <div class="card">
        <!-- inseriamo tramite le variabili del promps i dati dell'array d'oggetti -->
        <img :src="image" class="img_cards"> <!--indica il thumb che indica il link dell'immagine dell'oggetto-->
        <p>{{title.toUpperCase()}}</p> <!--indica il series che indica il titolo dell'immagine dell'oggetto-->
    </div>
    
</template>

<!-- parte style (css,scss ecc...) -->
<style  lang="scss" >
    .img_cards{
        width: 100%;
        height: 230px;               
        object-fit: cover;
        padding-bottom: 10px;  
        
        
        .img_cards :last-child{
            width: 10px;

        }
    }
        
    
    
</style>