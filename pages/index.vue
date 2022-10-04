<template>
  <div class="main">
    <Banner Page="Accueil" />
    <div class="bg-sable">

      <div class="container pt-4 text-center">
        <h2 class="color-wine mb-4"><b> Nos Prestations </b></h2>
        <div class="row mx-auto">

          <div class="col-sm-4 pb-4 px-3">
            <div class="card card-services">
              <img class="card-img-top" src="https://cdn.pixabay.com/photo/2017/02/16/13/42/box-2071537_1280.png" alt="services">
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


        <h2 class="color-wine mb-4"><b> Notre sélection de vins  </b></h2>
      </div> <!--fin container -->

    </div>
  </div>
  
</template>

<script>
export default {
  name: 'IndexPage'
}
  
</script>

<style scoped>
.card-services{
  width: 350px;
}
</style>
