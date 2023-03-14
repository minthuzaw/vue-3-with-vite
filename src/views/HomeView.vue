<script setup>
// import {ref} from 'vue';
import {useStorage} from "@/composables/useStorage";

let food = useStorage('food', 'pizza');

let obj = useStorage('obj', {one: 'one'});
setTimeout(() => {
  obj.value.one = "changed"
}, 2000);

// let food = ref(localStorage.getItem('food'))
// function write() {
//     localStorage.setItem('food', food.value);
// }
</script>

<template>
  <main>
    <p>
      What is your favorite food? <input type="text" v-model="food">
    </p>
  </main>
</template>
