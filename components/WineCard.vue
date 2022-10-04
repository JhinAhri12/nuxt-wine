<template>
    <div class="container">
        <div class="card m-3">
            <div class="row">
                <div class="col-sm-8">
                    <img src="../assets/banner.jpg" class="img-thumbnail m-2" alt="">
                </div>
                    <div class="col-sm-2">
                        <div class="card-body">
                            <p class="text-muted">Type</p>
                            <p>{{wine.</p>
                            <p class="text-muted">Years</p>
                            <p class="text-muted">Origin</p>
                        </div>
                    </div>
                    <div class="col-sm-2">
                        <div class="card-body">
                            <p class="text-muted">Capacity</p>
                            <p class="text-muted">Alcohol</p>
                        </div>
                    </div>
            </div>
            <h2>Nom</h2>
            <h3>Domaine</h3>
            <p><strong>Price</strong>&nbsp;<span>Contact</span>&nbsp;<span>Share</span></p>
            <hr>
            <p><span class="text-muted">Sale</span> <span class="text-muted">Reserve</span> <span class="text-muted">Arrived within</span></p>
            <hr>
            <button>Buy Now</button>
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