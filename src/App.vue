<script setup>
import { ref } from 'vue';
const count = ref(0);
const increment = () => {
  count.value++;
};
const reset = () => {
  count.value = 0;
};
</script>

<template>
  <div class="counter">
    <h2>Simple Counter</h2>
    <p class="count">Count: <span>{{ count }}</span></p>
    <div class="button">
      <button @click="increment">Increase Count</button>
      <button @click="reset">Reset Count</button>
    </div>
  </div>
</template>

<style scoped>
.counter {
  font-family: system-ui, sans-serif;
}
</style>
