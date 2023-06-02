<script setup lang="ts">

    defineProps<{ counter: number }>()
    
</script>

<template>
 <main>
    <h1>Counter: {{ counter }}</h1>
  </main>
</template>


<style scoped>
main{
  text-align: center;
}
</style>