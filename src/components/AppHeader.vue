<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            link: [
                { title: 'CHARACTERS',
                 
                },
                { title: 'COMICS',
                 
                },
                { title: 'MOVIE',
                  
                },
                { title: 'TV',
                  
                },
                { title: 'GAMES',
                  
                },
                { title: 'COLLECTIBLES',
                 
                },
                { title: 'VIDEO',
                 
                },
                { title: 'FANS',
                  
                },
                { title: 'NEWS',
                  
                },
                { title: 'SHOP',             
                },
                
            ],
        }
    },
    methods: {  
    }
}
</script>

<template>
   
   <section class="container d-flex justify-content-evenly align-items-center">    
        <!--LOGO-->
        <div>
            <img class="p-3" src="../assets/img/dc-logo.png" alt="">
        </div>
        
        <!--LINKS-->
        <ul class="d-flex gap-3">
            <li v-for="link in link" class="active">{{ link.title }}</li>     
        </ul>
   </section>

</template>

<style scoped lang="scss">
@use './style/generic' as *;
@use '../style/partials/variables' as *;

    li {
        height: 135px;
        display: flex;
        align-items: center;
        position: relative;

    &:hover.active::after {
       content:'';
       width: 100%;
       height: 3px;
       background-color: $brand-primary;
       position: absolute;
       bottom: 0;
    }
}

</style>
