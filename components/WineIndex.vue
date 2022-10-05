<template>
    <div class="col-sm-3 mb-5">
        <div class="card card-services">
        <h3 class="alert bg-wine ">{{wine.name}}</h3>
        <img :src="wine.img" class="card-img-top" :alt="wine.name"> 
            <div class="card-body">
                <p class="card-text">Lorem ipsum dolor .</p>
                <nuxt-link class="btn btn-switch-wine" :to="'/wine/' + wine.id">Voir les détails</nuxt-link>
            </div>
        </div> 
    </div>
     
</template>
<style scoped>
    img{
        height:200px;
        object-fit: cover;
       
    }
    a:hover{
        color: white;
    }
    h3{
        height: 100px;
        justify-content: center;
        display: flex;
        align-items: center;
    }
    .card-img, .card-img-top{
  border-top-left-radius : initial !important;
  border-top-right-radius : initial !important;
}
.alert {
  border-bottom-left-radius : initial !important;
  border-bottom-right-radius : initial !important;
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