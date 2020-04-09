<template>
    <div>
        <NewQuote/>
        <QuoteGrid :quotes="quotes"></QuoteGrid>
    </div>
</template>
<script>
    import QuoteGrid from "./QuoteGrid";
    import NewQuote from "./NewQuote";
  export default{
    name: "WonderfulQuotes",
    components:{
      QuoteGrid,
      NewQuote
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
