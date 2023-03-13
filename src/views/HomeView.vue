<script setup>
import TheWelcome from '../components/TheWelcome.vue'
import { ref } from "vue";

// eslint-disable-next-line no-undef
let message = $ref("Hello World!");
// let message = ref("Hello World!");
// setTimeout(() => {
//   message.value = "I have been changed!";
// }, 2000);

setTimeout(() => {
  message = "I have been changed!";
}, 2000);

let alertSomething = () => {
  alert("Do Something!")
};
</script>

<template>
  <main>
    <TheWelcome />
    <p>{{ message }}</p>
    <input type="text" v-model="message" />

    <button @click="alertSomething">Click</button>
  </main>
</template>
