<template>
  <div style="display: flex; flex-direction: column;justify-items: center;">
    <CustomButton @button-clicked="count = $event"></CustomButton>
    <div style="margin-top:10px">Number of times clicked : {{ count }}</div>
  </div>
</template>
<script setup>
import { ref } from "vue";
import CustomButton from './components/CustomButton.vue';

let count = ref(0);
</script>
