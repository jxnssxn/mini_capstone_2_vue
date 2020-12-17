<template>
  <div class="home">
    <h1>{{ message }}</h1>
    <div v-for="product in products">
    <h3>{{ product.name }}</h3>
    </div>
  </div>
</template>

<style>
</style>

<script>
import axios from "axios";
export default {
  data: function () {
    return {
      message: "Welcome to products index!",
      products: [],
      product: {},
    };
  },
  created: function () {
    this.productsIndex();
  },
  methods: {
    productsIndex: function () {
      console.log("products Index...print");
    },
  },
};
</script>
