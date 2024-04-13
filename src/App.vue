<script>
  import AppHeader from './components/AppHeader.vue';
  import ComicsList from './components/ComicsList.vue';
  import FeatureSection from './components/FeatureSection.vue';
  import AppFooter from './components/AppFooter.vue';
  import CardsProducts from './components/CardsProducts.vue';
  import Jumbotron from './components/Jumbotron.vue';


  export default {
    components: {
      AppHeader,
      Jumbotron,
      ComicsList,
      CardsProducts,
      FeatureSection,
      AppFooter,
    }
    }
  

</script>

<template>
 
    <AppHeader></AppHeader>
   
   
    <Jumbotron></Jumbotron>
   
      <main>

        <CardsProducts></CardsProducts>
         
        <ComicsList></ComicsList>

        <FeatureSection></FeatureSection>
      
      </main>

    
    <AppFooter></AppFooter>
  

</template>

<style lang="scss">
@use './style/generic' as *;
</style>












