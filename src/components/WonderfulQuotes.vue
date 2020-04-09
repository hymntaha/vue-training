<template>
    <div>
        <NewQuote @quoteAdded="newQuote"/>
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
    },
    methods:{
      newQuote(quote){
        return this.quote.push(quote)
      }
    }
  }
</script>
<style>

</style>
