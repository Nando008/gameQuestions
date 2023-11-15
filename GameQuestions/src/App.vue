
<script setup>
import { ref } from 'vue';


let num = ref('');

let array = ref([]);

function subir() {
  array.value.push(num.value)
}

</script>


<template>

  <input @keypress.enter="subir" v-model="num" type="text">
  <br>
  <p>{{ array }}</p>

</template>


<style scoped>



</style>
