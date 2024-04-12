<script>
 export default {
        name: 'AppFooter'
    }

</script>

<template>

  <section class="top-footer">

      <div class="ms-container">
       prova
    
     </div>


  </section>
  
  <section class="bottom-footer">footer</section>
  
</template>




<style scoped lang="scss">
 @use '../style/partials/variables' as *;



 .top-footer {
  background-image: url('../assets/img/footer-bg.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  color: white;

  .ms-container {
    height: 300px;
    background-image: url('../assets/img/dc-logo-bg.png');
    background-repeat: no-repeat;
    background-position: 100%;
    background-size: contain;
  }
 }

 .bottom-footer {
  background-color: $brand-secondary;
 }

</style>
