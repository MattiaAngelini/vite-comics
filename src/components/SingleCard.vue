<script>
 export default {
        name: 'SingleCard', 
        props: ['image','title']       
    }

</script>

<template>  
    
    <!--IMG & CARD from props-->
   <div class="ms-card">   
        <img class="p-1" :src="image">
        <div>{{ title }}</div>
   </div>

</template>

<style scoped lang="scss">
@use './style/generic' as *;

    .ms-card {
        color: white;

    img { width: 200px;
          height: 200px;
        
    }
}
    
</style>