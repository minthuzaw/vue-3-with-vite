<script setup>
// import TheWelcome from '../components/TheWelcome.vue'
import TheQuiz from "@/components/Quiz/TheQuiz.vue";
import { state } from "@/store/quizStore";
</script>

<template>
  <main>
<!--    <TheWelcome />-->
    <TheQuiz :quiz="state"/>
  </main>
</template>
