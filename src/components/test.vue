<!-- components/FormSelect.vue -->
<template>
    <div 
      class="flex items-center justify-between gap-5 px-4 text-sm relative"
      :class="{
            'bg-gray-100 py-2 rounded-md': theme == 'gray',
            'bg-gray-900 text-black rounded-xl py-2': theme == 'dark',
            'bg-primary text-black m-md-2 rounded-xl py-2': theme == 'primary'
      }"
    >
        <select
          v-model="filters"
          class="bg-transparent m-0 p-0 appearance-none w-full pr-5"
        >
            <slot />
        </select>

    </div>
</template>

<script setup>
import { ref } from 'vue';
  
const { theme } = defineProps(['theme']);
</script>
  