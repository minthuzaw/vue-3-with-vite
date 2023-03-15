<script setup>
import TabTextarea from "@/components/TabTextarea.vue";
import {ref} from "vue";

let comment = ref('text test');

setTimeout(()=>{
  comment.value = "changed";
}, 2000);
</script>

<template>
  <main>
    <TabTextarea v-model="comment" style="width: 100%; height: 300px"/>
  </main>
</template>
