<template>
  <div style="display: flex; flex-direction: column; align-items: center; justify-content: center;">
    {{ count }}
    <button @click="increment()">
      +
    </button>
  </div>
</template>

<script setup>
import {ref} from 'vue';

const count = ref(0);

function increment(){
  count.value++;
}
</script>

<style scoped>
</style>
