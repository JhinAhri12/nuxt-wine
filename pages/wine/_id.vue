<template>
    <div class="wine-details bg-sable">
        <Banner Page="Détails" />
        <WineCard :wine="wine" />
    </div>
    
</template>

<script>
export default {
      async asyncData({ $axios, error, params }) {
        try {
          const { data } = await $axios.get(
            'https://my-json-server.typicode.com/JhinAhri12/DBWine/wines/' + params.id
          )
          return {
            wine: data
          }
        } catch (e) {
          error({
            statusCode: 503,
            message: 'Unable to fetch wine #' + params.id
          })
        }
      }
}
</script>
