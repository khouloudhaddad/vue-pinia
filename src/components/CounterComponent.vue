<script setup lang="ts">
import { ref } from 'vue';
const counter = ref(0)

const emit = defineEmits(['increment'])

const increment = () => {
    
    counter.value++;
    emit('increment', counter.value)

}

</script>

<template>
    <button @click="increment">Increment {{ counter }}</button>
</template>


<style scoped>
main{
  text-align: center;
}
</style>