<!--
This example demonstrates handling user input with the v-on directive.
-->

<script>
export default {
  data() {
    return {
      message: 'yeet'
    }
  },
  methods: {

    pushMessage(){
      
    }

  }
}
</script>

<template>
  <input v-model="message" placeholder="edit me"><br>
  <button @click="pushMessage()">send message to server</button><br>
  <p>Message is: {{ message }}</p>
</template>

<style>
button, a {
  display: block;
  margin-bottom: 1em;
}
</style>