<template>
    <div>
        <NewQuote @quoteAdded="newQuote"/>
        <QuoteGrid :quotes="quotes" @quoteDeleted="deleteQuote"></QuoteGrid>
        <div class="row">
            <div class="col-sm-12 text-center">
                <div class="alert alert-info">Info: Click on a quote to delete it!</div>
            </div>
        </div>
    </div>
</template>
<script>
    import QuoteGrid from "./QuoteGrid";
    import NewQuote from "./NewQuote";
    import Header from './Header';
  export default{
    name: "WonderfulQuotes",
    components:{
      QuoteGrid,
      NewQuote,
      Header
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
         this.quote.push(quote)
      },
      deleteQuote(index) {
         this.quotes.splice(index,1)
      }
    }
  }
</script>
<style>

</style>
