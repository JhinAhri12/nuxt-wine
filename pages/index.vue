<template>
  <div class="main">
    <Banner Page="Accueil" />
    <div class="bg-sable">

      <div class="container pt-4 text-center">
        <h2 class="color-wine mb-4"><b> Nos Prestations </b></h2>
        <div class="row mx-auto">

          <div class="col-sm-4 pb-4 px-3">
            <div class="card card-services">
              <img class="card-img-top wine-img" src="https://cdn.pixabay.com/photo/2015/11/06/12/52/roller-1027345__480.jpg" alt="services">
              <div class="card-body">
                <h3 class="card-title">Livraison</h3>
                <a href="#" class="btn btn-wine">Se faire livrer</a>
              </div>
            </div>
          </div>

          <div class="col-sm-4 pb-4 px-3">
            <div class="card card-services">
              <img class="card-img-top" src="https://cdn.pixabay.com/photo/2017/06/10/07/18/list-2389219_1280.png" alt="services">
              <div class="card-body">
                <h3 class="card-title">Conseil</h3>
                <a href="#" class="btn btn-wine">Appeller nos conseillers</a>
              </div>
            </div>
          </div>

          <div class="col-sm-4 pb-4 px-3">
            <div class="card card-services">
              <img class="card-img-top" src="https://cdn.pixabay.com/photo/2021/04/16/12/38/online-store-6183487_1280.png" alt="services">
              <div class="card-body">
                <h3 class="card-title">Boutique en ligne</h3>
                <a href="#" class="btn btn-wine">Voir nos produits</a>
              </div>
            </div>
          </div>

        </div> <!-- fin row -->

        <div class="container pt-4 text-center">
          <h2 class="color-wine mb-4"><b> Notre sélection de vins </b></h2>
          <div class="row mx-auto">
 

            <WineIndex
              v-for="(wine, id) in wines"
              :key="id"
              :wine="wine"
              :data-index="id"
            />
          </div>
        </div>
      </div> <!--fin container -->

    </div>
  </div>
  
</template>

<script>
import WineIndex from '@/components/WineIndex.vue'
export default {
  name: 'IndexPage',
  data(){
    return {
      wines: ''
    };
  },
  async asyncData({ $axios, error }) {
        try {
          const { data } = await $axios.get(
            'https://my-json-server.typicode.com/JhinAhri12/DBWine/wines?_limit=4'
                      )
          return {
            wines: data
          }
        } catch (e) {
          error({
            statusCode: 503,
            message: 'Unable to fetch wine '
          })
        }
      },
  components: {
    WineIndex
  },
} 
  
</script>

<style scoped>
.card-services{
  width: 350px;
}


</style>
