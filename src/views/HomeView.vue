<script>
import flash from '@/mixins/flash';

export default {
  mixins: [flash]
}
</script>

<template>
  <main>
    <button @click="flash('It is work on home view.')">Click me</button>
  </main>
</template>
