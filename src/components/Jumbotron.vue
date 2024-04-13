<script>
 export default {
        name: 'Jumbotron',       
    }
</script>

<template>
        <!--CONTAINER IMG WRAP-->
        <div class="container-jumbotron"></div>
</template>

<style scoped lang="scss">
@use './style/generic' as *;

    .container-jumbotron {
        height: 300px;
        width: 100%;
        background-image: url('../assets/img/jumbotron.jpg');
        background-size: cover; 
}
   
</style>