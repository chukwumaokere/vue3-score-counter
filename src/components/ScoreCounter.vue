<template>
  <div>
    <h2>{{name}} #{{number}}</h2>
    <p> {{player.score}} </p>
    <button @click="player.score--">Decrease</button>
    <button @click="player.score++">Increase</button>
  </div>
</template>

<script setup="props">
import { reactive } from 'vue'

 export default{
    props: {
        name: String,
        number: Number,
    },
    inheritAttrs: false,
 }
 //export const name = props.name;
  export const player = reactive({
    score: 0,
  });
  
</script>

<style>

</style>