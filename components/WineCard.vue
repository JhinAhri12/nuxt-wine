<template>
    <div class="container">
        <div class="card m-3">
            <div class="row">
                <div class="col-sm-6 div-wine">
                    <img :src="wine.img" class="img-thumbnail mb-2 img-wine" alt="">
                </div>
                    <div class="col-sm-3">
                        <div class="card-body">
                            <p class="text-muted">Type</p>
                            <p>{{wine.type}}</p>
                            <p class="text-muted">Millésime</p>
                            <p>{{wine.years}}</p>
                            <p class="text-muted">Origine</p>
                            <p>{{wine.origin}}</p>
                        </div>
                    </div>
                    <div class="col-sm-3">
                        <div class="card-body">
                            <p class="text-muted">Capacité</p>
                            <p>{{wine.capacity}}</p>
                            <p class="text-muted">Degré d'alcool</p>
                            <p>{{wine.alcohol}}</p>
                        </div>
                    </div>
            </div>
            <div class="text-center">

            
            <h2 class="color-wine">{{wine.name}}</h2>
            <h3 class="text-muted mb-4">{{wine.domaine}}</h3>
            <p class="mb-5"><strong>Prix</strong> {{wine.price}}&nbsp;<span class="f-right"><button class="btn btn-wine">Contact</button>&nbsp;<button class="btn btn-wine">Partager</button></span></p>
            <hr>
            <p ><span class="text-muted">Nombre de ventes</span> {{wine.sale}} <span class="text-muted">Réserve</span> {{wine.reserve}} <span class="text-muted">Livraison à partir de</span> {{wine.date}}</p>
            <hr>
            </div>
            <div class="container text-center mb-3">
                <button class="btn btn-wine">Acheter</button>
            </div>
            
        </div>
        
        
    </div>
</template>
<style scoped>
.div-wine{
    display: flex;
    justify-content: center;
    align-items: center;
}
.f-right{
    float:right;
    margin-right: 150px;
}
.img-wine{
    height: 200px !important;
    width: 400px !important;
    object-fit: cover;
}
</style>
<script>
export default {
    name: 'WineCard',
    props: {
        wine: Object
      }
}
</script>