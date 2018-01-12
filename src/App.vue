<template>
  <div class="container">
    <app-new-quote @quoteAdded="newQuote"></app-new-quote>
    <app-quote-grid :quotes="quotes"></app-quote-grid>
  </div>
</template>

<script>
  import QuoteGrid from "./components/QuoteGrid.vue";
  import NewQuote from "./components/NewQuote.vue";
  export default {
    data: function() {
      return {
        quotes: [
          "Just a Quote to see something",
          "Nam fugit possimus voluptas explicabo quia debitis omnis qui.",
          "Odit delectus libero repudiandae earum dolorem in corrupti quis."
        ],
        maxQuotes: 10
      };
    },
    methods: {
      newQuote(quote) {
        this.quotes.push(quote);
      }
    },
    components: {
      appQuoteGrid: QuoteGrid,
      appNewQuote: NewQuote,
      // appHeader: Header
    }
  };
</script>

<style>
  
</style>
