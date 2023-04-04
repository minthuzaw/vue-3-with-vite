<template>
  <QuizHeader />
<!--  <QuizQuestion />-->

  <QuizFooter :quiz="quiz"/>
</template>

<script setup>
import QuizHeader from "@/components/Quiz/QuizHeader.vue";
// import QuizQuestion from "@/components/Quiz/QuizQuestion.vue";
import QuizFooter from "@/components/Quiz/QuizFooter.vue";
import { provide } from "vue";

let props = defineProps({quiz: Object});

// eslint-disable-next-line no-undef
provide('quiz', props.quiz)
/*let name = ref('John');
provide('name', {
  name,
  changeName: () => name.value = 'The name has been changed.'
});*/

</script>
