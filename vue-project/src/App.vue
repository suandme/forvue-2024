<script setup>
import {ref}  from 'vue'
const num = ref(1)
const mes = ref('')

function clickMe()
{
  num.value++
  if (num.value==10)
  {
     mes.value='加油!'
  }else if (num.value==20)
  {
     mes.value='再加油!'
  }
}

</script>

<template>
  <div >
    {{num}} {{mes}}
    <button  type="button" v-on:click="clickMe">點我</button>
  </div>
</template>