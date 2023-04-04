<template>
  <div>
    <h1>{{ state.name }}</h1>

    <p>Welcome to first quiz.</p>
  </div>
</template>

<script setup>
import {state} from "@/store/quizStore";
</script>
