<!--
This example demonstrates handling user input with the v-on directive.
-->

<script setup>
  import { reactive } from 'vue'

  import Header1 from './components/header.vue'


  const number = reactive({count:0})

  function increment(){
    number.count++
  }
  function reset(){
    number.count = 0
  }

</script>

<template>
  <Header1 />
  <button @click="increment()">add one</button><br>
  <button @click="reset()">reset</button>
  <p>count is {{ number.count }}</p>
</template>

<style>

body{
  margin:0px;
  padding:0px
}

button, a {
  display: block;
  margin-bottom: 1em;
}


</style>