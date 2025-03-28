<script setup lang="ts">
import { Button } from './ui/button';

defineProps<{
  msg: string
}>()
</script>

<template>
  <div class="greetings">
    <p class="text-3xl font-bold underline text-red-900">Tailwind installed</p>
    <Button variant="secondary">This is a button</Button>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {

  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
