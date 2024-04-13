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

  <!---------------TOP FOOTER - LIST----------------->
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
  
  <!--------------BOTTOM FOOTER - SIGN UP & SOCIAL LOGO---------------->

  <section class="bottom-footer p-3">
    <div class="container d-flex align-items-center justify-content-between">
      <div class="border border-primary p-2"><span>SIGN UP NOW</span></div>
        <div class="d-flex align-items-center gap-3">
      
           <div class="ms-title"><span>FOLLOW US</span></div>    
           <div v-for="icon in socialLogo ">
             <img class="p-2" :src="'src/assets/img/' + icon.image" alt="">      
        </div>

      </div>
    </div>
  </section>

</template>

<style scoped lang="scss">
 @use '../style/partials/variables' as *;
  
  /******TOP FOOTER *****/
  .top-footer {
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    color: grey;

    h6{color: white;}

    .ms-container {
      background-image: url('../assets/img/dc-logo-bg.png');
      background-repeat: no-repeat;
      background-position: 100%;
      background-size: contain;
      font-size: 14px;

    }
  }
  
  /******BOTTOM FOOTER *****/
  .bottom-footer {
    background-color: $brand-secondary;
    color: white;
    font-weight: 600;

    .ms-title {
      color: $brand-primary;

    }
  }

</style>
