<template>
  <div>
    <h5>{{ state.name }}</h5>
    <button @click="state.name = 'A new quiz'">Change Name</button>

    <ul>
      <li><a href="#">Got a Job</a></li>
      <li><a href="#">Contact Us</a></li>
    </ul>
  </div>
</template>

<script setup>
import {state} from "@/store/quizStore";

</script>
