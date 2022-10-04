<template>
    <div class="col-sm-3 mb-5">
        <div class="card card-services">
        <h3>{{wine.name}}</h3>
        <img :src="wine.img" class="card-img-top" :alt="wine.name"> 
        <div class="card-body">
            <p class="card-text">Lorem ipsum dolor .</p>
            <nuxt-link :to="'/wine/' + wine.id"><a class="btn btn-wine">Voir les détails</a></nuxt-link>
        </div>
    </div> 
    </div>
     
</template>
<style scoped>
    img{
        height:200px;
        object-fit: cover;
       
    }
</style>
 <script>
    export default {
      name: 'WineIndex',
      props: {
        wine: Object
      }
    }
</script>