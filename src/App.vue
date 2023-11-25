<template>
  <div style="display: flex; flex-direction: column; align-items: center; justify-content: center; gap: 20px;">
    <q-card
      dark
      bordered
      class="bg-grey-6 my-card"
    >
      <q-card-section class="section-card">
        {{ count }}
      </q-card-section>
    </q-card>
    <q-btn
      @click="increment()"
      color="#ffffff"
      text-color="black"
      label="Increment"
    />
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
.section-card {
  padding: 10px 20px;
}
</style>
