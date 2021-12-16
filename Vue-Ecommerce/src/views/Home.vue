<template>
  <div class="home-component">
    <div class="jumbotron jumbotron-fluid">
      <div class="container">
        <img alt="MEN FORM logo" src="../assets/logo.png" width="200px" />
        <p class="lead">An ecommerce store for all your clothing needs</p>
        <h3 class="display-5 ">
          <span>Upto 50% off</span>
        </h3>
        
      </div>
    </div>
    <nav aria-label="breadcrumb">
      <ol class="breadcrumb">
        <li class="breadcrumb-item active" aria-current="page">
          Our Best Products
        </li>
        <li class="ml-auto" aria-current="page">
          <router-link to="/products" class="white">Show all products</router-link>
        </li>
      </ol>
    </nav>
    <BestProducts></BestProducts>
    <nav aria-label="breadcrumb">
      <ol class="breadcrumb">
        <li class="breadcrumb-item active" aria-current="page">
          Our Top Products
        </li>
        <li class="ml-auto" aria-current="page">
          <router-link to="/products" class="white">Show all</router-link>
        </li>
      </ol>
    </nav>
    <TopProducts></TopProducts>
  </div>
</template>

<script>
// @ is an alias to /src

import BestProducts from "@/components/products/BestProducts.vue";
import TopProducts from "@/components/products/TopProducts.vue";
export default {
  name: "home",
  components: {
    BestProducts,
    TopProducts,
  },
};
</script>
<style>
.jumbotron {
  padding: 1rem 0rem;
}
</style>
