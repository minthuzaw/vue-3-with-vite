<script setup>
// import TheWelcome from '../components/TheWelcome.vue'
import Quiz from "@/components/Quiz/Quiz.vue";
</script>

<template>
  <main>
<!--    <TheWelcome />-->
    <Quiz :quiz="{name: 'My First Quiz', question: []}"/>
  </main>
</template>
