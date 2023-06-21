<!-- parte logica (javascript) -->
<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppJumbotron from './components/AppJumbotron.vue';
export default {
  components:{
    AppHeader,
    AppMain,
    AppFooter,
    AppJumbotron
  }
  
}
</script>
<!-- parte grafica (html) -->
<template lang="">
  <div>
    <!-- inserite le componenti -->
    <AppHeader/>
    <AppJumbotron/>
    <AppMain/>
    <AppFooter/>
    
  </div>
</template>
<!-- parte di style (scss) -->
<style lang="scss">
  *{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
  
</style>