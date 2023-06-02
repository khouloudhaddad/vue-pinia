<script setup lang="ts">
import  CounterComponent from '@/components/CounterComponent.vue';
import PrintComponent from '@/components/PrintComponent.vue';
import { ref } from 'vue';

const counter = ref(0)
const updateSate = (value: number) => {
  counter.value = value
}
</script>

<template>
 <main>
  {{ counter }}
   <print-component :counter="counter" />
   <counter-component @increment="updateSate" />
  </main>
</template>


<style scoped>
main{
  text-align: center;
}
</style>