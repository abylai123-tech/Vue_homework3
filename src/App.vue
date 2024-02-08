<template>
  <div>
    <h1>Hello world!</h1>
    <input type="text" v-model="login" placeholder="login" />
    <input type="text" v-model="password" placeholder="password" />
    <input type="text" v-model="email" placeholder="email" />
    <input type="text" v-model="phoneNumber" placeholder="phone number" />

    <button @click="handleButtonClick">Click me</button>
    <p>{{ userData }}</p>
  </div>
</template>

<script setup>
import { ref } from "vue";

const login = ref("");
const password = ref("");
const email = ref("");
const phoneNumber = ref("");
const userData = ref("");

const handleButtonClick = () => {
  userData.value = `Login: ${login.value}, Password: ${password.value}, Email: ${email.value}, Phone Number: ${phoneNumber.value}`;
};
</script>

<style scoped>
h1 {
  color: red;
}
</style>
