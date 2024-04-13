<script>
 export default {
        name: 'SingleCard', 
        props: ['image','title']       
    }

</script>

<template>  
    
   <div class="ms-card">   
        <img :src="image">
        <div>{{title}}</div>
   </div>

</template>

<style scoped lang="scss">

.ms-card {
    color: white;

    img { width: 200px;
          height: 200px;
        
    }
}
    
</style>