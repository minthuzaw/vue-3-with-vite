<script setup>
import {useFlash} from "@/composables/useFlash"

let { flash } = useFlash();
</script>

<template>
  <div>
    <button @click="flash('Success', 'It is work from contact view.', 'error')">Click me</button>
  </div>
</template>
