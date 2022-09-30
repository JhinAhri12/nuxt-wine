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