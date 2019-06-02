<template>
  <div>
    <h1>The Stocks Component</h1>
    <app-stock v-for="stock in stocks" :stock="stock"></app-stock>
  </div>
</template>

<script>
import stock from "./Stock.vue";

export default {
  data() {
    return {
      stocks: [
        { id: 1, name: "BMW", price: 110 },
        { id: 2, name: "Google", price: 210 },
        { id: 3, name: "FB", price: 180 },
        { id: 4, name: "Twitter", price: 5 }
      ]
    };
  },
  components: {
    appStock: stock
  }
};
</script>

