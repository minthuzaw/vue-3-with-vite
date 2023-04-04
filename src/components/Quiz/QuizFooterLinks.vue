<template>
  <div>
    <h5>{{ quiz.name }}</h5>
<!--    <p>{{ name }}</p>
    <button @click="changeName">Change Name</button>-->

    <ul>
      <li><a href="#">Got a Job</a></li>
      <li><a href="#">Contact Us</a></li>
    </ul>
  </div>
</template>

<script setup>
import {inject} from "vue";

defineProps({quiz: Object});

let quiz = inject('quiz')

// let {name, changeName} = inject('name');
</script>
