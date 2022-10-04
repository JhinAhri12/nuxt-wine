<template>
    <div class="container">
        <div class="card m-3">
            <div class="row">
                <div class="col-sm-8">
                    <img :src="wine.img" class="img-thumbnail m-2" alt="">
                </div>
                    <div class="col-sm-2">
                        <div class="card-body">
                            <p class="text-muted">Type</p>
                            <p>{{wine.type}}</p>
                            <p class="text-muted">Years</p>
                            <p>{{wine.years}}</p>
                            <p class="text-muted">Origin</p>
                            <p>{{wine.origin}}</p>
                        </div>
                    </div>
                    <div class="col-sm-2">
                        <div class="card-body">
                            <p class="text-muted">Capacity</p>
                            <p>{{wine.capacity}}</p>
                            <p class="text-muted">Alcohol</p>
                            <p>{{wine.alcohol}}</p>
                        </div>
                    </div>
            </div>
            <div class="text-center">

            
            <h2>{{wine.name}}</h2>
            <h3>{{wine.domaine}}</h3>
            <p><strong>Price</strong> {{wine.price}}&nbsp;<span><btn class="btn btn-wine">Contact</btn>&nbsp;<btn class="btn btn-wine">Partager</btn></span></p>
            <hr>
            <p><span class="text-muted">Sale</span> {{wine.sale}} <span class="text-muted">Reserve</span> {{wine.reserve}} <span class="text-muted">Arrived within</span> {{wine.date}}</p>
            <hr>
            </div>
            <div class="container text-center mb-3">
                <btn class="btn btn-wine">Acheter</btn>
            </div>
            
        </div>
        
        
    </div>
</template>
<script>
export default {
    name: 'WineCard',
    props: {
        wine: Object
      }
}
</script>