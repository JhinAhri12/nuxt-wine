<template>
    <div id="carouselControls" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-inner">
            <div class="carousel-item active">
            <img src="./../assets/wine1.jpg" class="d-block w-100" alt="wine">
            </div>
            <div class="carousel-item">
            <img src="./../assets/wine2.jpg" class="d-block w-100" alt="wine">
            </div>
            <div class="carousel-item">
            <img src="./../assets/wine3.jpg" class="d-block w-100" alt="wine">
            </div>
        </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselControls" data-bs-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselControls" data-bs-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
    </button>
    </div>
</template>
<script>
export default {
  name: 'Carousel'
}
</script>