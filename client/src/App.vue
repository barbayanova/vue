<template>
    <h1>
    Проект на Vue
   <button @click="increment">Счетчик {{ counter2}} </button>
    </h1>
</template>
<script setup>
import { onMounted, ref } from 'vue'
const counter = ref(0)

function increment () {
    counter.value++
}
onMounted(() => {
    console.log(counter);
    
})

console.log(counter);
console.log(counter2);
</script>
