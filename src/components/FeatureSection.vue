<script>
 export default {
        name: 'FeatureSection',

        data() {
        return {
            cards: [
                { title: 'DIGITAL COMICS',
                  image: 'buy-comics-digital-comics.png'
                },
                { title: 'DC MERCHANDISE',
                  image: 'buy-comics-merchandise.png'
                },
                { title: 'SUBSCRIPTION',
                  image: 'buy-comics-subscriptions.png'
                },
                { title: 'COMIC SHOP LOCATOR',
                  image: 'buy-comics-shop-locator.png'
                },
                { title: 'DC POWER VISA',
                  image: 'buy-dc-power-visa.svg'
                }
                
            ],
        }
    }

    }
    
</script>

<template>

   <section class="feat-section ">

    <ul class="d-flex gap-3 justify-content-center align-items-center m-0 p-2">      
     
        <li  v-for="card in cards">
            <img class="p-3" :src="'src/assets/img/' + card.image" alt="">
            {{ card.title }}
        </li> 
    </ul>

   </section>
  
</template>


<style scoped lang="scss">
 
 @use '../style/partials/variables' as *;

 .feat-section {
    background-color: $brand-primary;
    color: white;
   
   
    img {
        height: 80px;
    }
 }


</style>
