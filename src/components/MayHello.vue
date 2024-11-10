<script setup>
import { ref } from 'vue'
const count = ref(0)

function increment() {
    count.value++
}

// function updateCount(e) {
//     count.value = Number(e.target.value)
// }

// export default {
//     data() {
//         return {
//             count: 0
//         }
//     },
//     methods: {
//         increment() {
//             this.count++
//         }
//     }
// }

</script>


<template>
  <h1>{{count}}</H1>
  <button @click="increment">+</button>
  <input v-model="count" />
</template>

