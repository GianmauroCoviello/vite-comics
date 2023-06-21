<script>

export default {
    props:{
        image: String
    }
    
    
}
</script>

<template lang="">
    <div class="card">
        <img :src="image" class="img_cards">
        
    </div>
    
</template>

<style >
    .img_cards{
        width: 100%;
        height: 200px;               
        object-fit: cover;
                               
    }
        
    
    
</style>