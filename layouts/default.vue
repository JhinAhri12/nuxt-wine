<template>
    <div id="app">
        <Header />
       
        <nuxt />

        <WineFooter />
    </div>
</template>
<script>
import WineFooter from "@/components/WineFooter.vue";
import Header from "@/components/Header.vue";
export default {
    components: {
        Header,
        WineFooter
    }
}
</script>

<style>
.btn-wine{
    color: white;
    padding: 8px 24px;
    border-radius: 4px;
    background: #a54952;
    transition: background 0.3s ease;
}
.btn-wine:hover {
  background-color: #ad2533;
  color: white;
}

.color-wine{
    color: #ad2533;
}
.bg-sable{
    background-color: rgba(251, 243, 229, 0.25);
}
.bg-wine{
    background-color: #a54952;
    color: white;
}
.btn-switch-wine{
    background-color: white;
    color: #ad2533;
    border: 1px solid #ad2533;
}
.btn-switch-wine:hover{
    background-color: #ad2533;
    border: 1px solid white;
}
.bg-nav{
    background-color: #8b3e46 !important;
}
</style>

