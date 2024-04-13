<script>
 export default {
        name: 'SingleCard', 
        props: ['image','title']       
    }

</script>

<template>

    <img :src="image">
    <h5>{{title}}</h5>
    
</template>

<style scoped lang="scss">


</style>