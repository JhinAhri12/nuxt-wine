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
</style>

