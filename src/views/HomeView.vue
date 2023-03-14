<script setup>
import {ref} from 'vue';

let food = ref(localStorage.getItem('food'))

function write() {
    localStorage.setItem('food', food.value);
}
</script>

<template>
  <main>
    <p>
      What is your favorite food? <input type="text" v-model="food" @input="write">
    </p>
  </main>
</template>
