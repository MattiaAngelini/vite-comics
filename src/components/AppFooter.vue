<script>
 export default {
        name: 'AppFooter',
        data() {
        return {
            socialLogo: [
                { title: 'facebook',
                  image: 'footer-facebook.png'
                },
                { title: 'twitter',
                  image: 'footer-twitter.png'
                },
                { title: 'youtube',
                  image: 'footer-youtube.png'
                },
                { title: 'pinterest',
                  image: 'footer-pinterest.png'
                },
                { title: 'maps',
                  image: 'footer-periscope.png'
                }
                
            ],
        }
    }
    }

</script>

<template>

  <section class="top-footer">

    <div class="ms-container container d-flex align-items p-4">

      <div>

        <ul class="m-0">
          <h6>DC ComicsList</h6>
          <li>Characters</li>
          <li>Characters</li>
          <li>Characters</li>
          <li>Characters</li>
          <li>Characters</li>
          <li>Characters</li>
          <li>Characters</li>
        </ul>


        <ul class="mt-2">
          <h6>DC ComicsList</h6>
          <li>Characters</li>
          <li>Characters</li>
          <li>Characters</li>
        </ul>
      </div>

      <ul class="m-0">
        <h6>DC ComicsList</h6>
        <li>Characters</li>
        <li>Characters</li>
        <li>Characters</li>
        <li>Characters</li>
        <li>Characters</li>
        <li>Characters</li>
        <li>Characters</li>
        <li>Characters</li>
        <li>Characters</li>
        <li>Characters</li>
      </ul>


      <ul class="m-0">
        <h6>DC ComicsList</h6>
        <li>Characters</li>
        <li>Characters</li>
        <li>Characters</li>
      </ul>


    </div>

  </section>

  <section class="bottom-footer ">

    <div class="container d-flex justify-content-between">

    <div><span>SIGN UP NOW</span></div>

    <div class="d-flex gap-3">
      <div><span>FOLLOWUS</span></div>
      

      <div v-for="icon in socialLogo ">
        <img :src="'src/assets/img/' + icon.image" alt="">
      
      </div>
    </div>


  </div>
  
  </section>

</template>


<style scoped lang="scss">
 @use '../style/partials/variables' as *;



 .top-footer {
  background-image: url('../assets/img/footer-bg.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  color: white;

  .ms-container {
    background-image: url('../assets/img/dc-logo-bg.png');
    background-repeat: no-repeat;
    background-position: 100%;
    background-size: contain;
    font-size: 14px;

    
  }
 }

 .bottom-footer {
  background-color: $brand-secondary;
  color: white;
 }

</style>
