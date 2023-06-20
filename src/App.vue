<!-- parte logica (javascript) -->
<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
export default {
  components:{
    AppHeader,
    AppMain,
    AppFooter,
  }
  
}
</script>
<!-- parte grafica (html) -->
<template lang="">
  <div>
    <AppHeader/>
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