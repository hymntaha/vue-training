<template>
    <div>
        <QuoteGrid :quotes></QuoteGrid>
    </div>
</template>
<script>
    import QuoteGrid from "./QuoteGrid";
  export default{
    name: "WonderfulQuotes",
    components:{
      QuoteGrid
    },
    data: function(){
      return{
        quotes: [
          'Just a Quote to see something'
        ],
        maxQuotes: 10
      }
    }
  }
</script>
<style>

</style>
