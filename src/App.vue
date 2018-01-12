<template>
  <div class="container">
    <app-quote-grid :quotes="quotes"></app-quote-grid>
  </div>
</template>

<script>
  import QuoteGrid from "./components/QuoteGrid.vue";
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
    components: {
      appQuoteGrid: QuoteGrid,
    //  appNewQuote: NewQuote,
     // appHeader: Header
    }
  };
</script>

<style>
  
</style>
