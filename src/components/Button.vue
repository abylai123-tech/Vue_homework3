<template>
    <button :style="{ backgroundColor: buttonColor }">
      {{ buttonText }}
    </button>
  </template>
  
  <script>
  export default {
    props: {
      buttonText: {
        type: String,
        required: true
      },
      buttonColor: {
        type: String,
        required: true
      }
    },
  };
  </script>
  
  <style scoped>
  button {
    padding: 0.5rem 1rem;
    color: #fff;
    border: none;
    cursor: pointer;
  }
  </style>
  