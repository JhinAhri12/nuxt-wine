<template>
    <div class="banner" style="background-image: linear-gradient(rgba(0,0,0,0.4),rgba(0,0,0,0.4)),url(https://cdn.pixabay.com/photo/2018/11/24/13/29/white-wine-3835585_1280.jpg)">
    
        <div class="container">
            <p><strong>{{Page}}</strong></p>
        </div>
    </div>

</template>
<script>
export default {
    name: 'Banner',
    props: { Page: String } 
}
</script>
<style scoped>
p{
    text-align: center;
    color:white;
}
.banner {
  background-size: cover;
  background-position: center;
  padding: 150px 0;
  
}

.banner h1 {
  margin: 0;
  color: white;
  text-shadow: 1px 1px 3px rgba(0,0,0,0.2);
  font-size: 32px;
  font-weight: bold;
}

.banner p {
  font-size: 20px;
  color: white;
  opacity: .7;
  text-shadow: 1px 1px 3px rgba(0,0,0,0.2);
}
</style>