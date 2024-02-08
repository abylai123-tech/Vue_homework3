<template>  
      <div class="product-card">
        <h2>{{ productName }}</h2>
        <p>{{ description }}</p>
        <div class="price">{{ price }}</div>
      </div>
  </template>
  
  <script>
  
  export default {
    props: {
        productName: {
          type: String,
          required: true
        },
        description: {
          type: String,
          required: true
        },
        price: {
          type: String,
          required: true
        }
    }
  };
  </script>
  
  <style scoped>
  .product-card {
    border: 1px solid #ccc;
    padding: 1rem;
    margin: 1rem;
  }
  </style>
  