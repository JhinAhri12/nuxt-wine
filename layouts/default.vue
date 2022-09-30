<template>
    <div id="app">
        <div class="container">
            <nuxt />
        </div>
        <WineFooter />
    </div>
</template>
<script>
import WineFooter from "@/components/WineFooter.vue";
export default {
    components: {
        WineFooter
    }
}
</script>