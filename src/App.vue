<script>
  import AppHeader from './components/AppHeader.vue';
  import ComicsList from './components/ComicsList.vue';
  import FeatureSection from './components/FeatureSection.vue';
  import AppFooter from './components/AppFooter.vue';


  export default {
    components: {
      AppHeader,
      ComicsList,
      FeatureSection,
      AppFooter,
    }
  }

</script>

<template>
 
    <AppHeader></AppHeader>
   
      <main>
        <ComicsList></ComicsList>

        <FeatureSection></FeatureSection>
      </main>
    
    <AppFooter></AppFooter>
  
</template>

<style lang="scss">
@use './style/generic' as *;
</style>
