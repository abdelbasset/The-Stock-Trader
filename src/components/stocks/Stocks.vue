<template>
  <div class="container">
    <h1>The Stocks Component</h1>
    <app-stock v-for="stock in stocks" :stock="stock"></app-stock>
  </div>
</template>

<script>
import stock from "./Stock.vue";

export default {
  components: {
    appStock: stock
  },
  computed : {
    stocks(){
      return this.$store.getters.stocks;
    }
  }
};
</script>

