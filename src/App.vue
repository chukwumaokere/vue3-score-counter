<template>
  <ScoreCounter name="Lou" />
  <ScoreCounter name="Christina" />
</template>

<script>
import ScoreCounter from './components/ScoreCounter'

export default{
  components:{
    ScoreCounter,
  }
}
</script>

<style>
#app{
  text-align: center;
  font-size: 3rem;
  font-family: sans-serif;
}
</style>
