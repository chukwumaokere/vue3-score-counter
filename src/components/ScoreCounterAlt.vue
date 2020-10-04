<template>
  <div>
    <h2>{{name}}</h2>
    <p> {{player.score}} </p>
    <button @click="player.score--">Decrease</button>
    <button @click="player.score++">Increase</button>
  </div>
</template>

<script>
import { reactive } from 'vue'
 export default{
    props: {
        name: String,
    },
    inheritAttrs: false,
    setup(props){
        const player = reactive({
            score: 0,
        });
        return {
            player,
            playerName: props.name,
        }
    }
 }
</script>

<style>

</style>