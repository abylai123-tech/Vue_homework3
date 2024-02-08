<template>
    <header>
      <h1>{{ title }}</h1>
    </header>
</template>
  
  <script>
  export default {
    props: {
      title: {
        type: String,
        required: true
      }
    }
  };
  </script>
  
  <style scoped>
  header {
    background-color: #3498db;
    color: #fff;
    padding: 10px;
    text-align: center;
  }
  </style>  