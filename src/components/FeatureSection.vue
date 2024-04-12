<script>
 export default {
        name: 'AppMain',

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

   <section class="feat-section d-flex gap-3 justify-content-center align-items-center m-0">

    <ul v-for="card in cards">      
        <li>{{ card.title }}</li>
        <li><img :src="'src/assets/img/' + card.image" alt=""></li> 
    </ul>

   </section>
  
</template>


<style scoped lang="scss">
 
 @use '../style/partials/variables' as *;

 .feat-section {
    background-color: $brand-primary;
 }

</style>
