<!-- App.vue -->
<template>
  <test2></test2>
  <test3></test3>

  <FormSelect v-model="selectedOption" theme="dark">
    <option class="bg-white m-0" value="">Toutes les activitiés</option>
    <option class="bg-white m-0">1</option>
    <option class="bg-white m-0">2</option>
    <option class="bg-white m-0">3</option>
    <option class="bg-white m-0">4</option>
  </FormSelect>

</template>

<script setup>
import { ref } from 'vue';
import FormSelect from './components/test.vue';
const selectedOption = ref('');

import test2 from './components/test2.vue';
</script>
