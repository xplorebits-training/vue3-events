<template>
  <button @click="onClickButton">CLICK HERE</button>
</template>
<style scoped>
button{
  padding: 4px 10px;
  border-radius: 6px;
  background-color: lightgray;
}
button:hover{
  background-color: white;
 
}
</style>
<script setup>
let count = 0;
const emits = defineEmits(["button-clicked"]);

const onClickButton = function(){
  count += 1;
  emits("button-clicked",count)
}
</script>