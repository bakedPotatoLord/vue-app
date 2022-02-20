<!--
This example demonstrates handling user input with the v-on directive.
-->

<script>
export default {
  data() {
    return {
      message: 'Hello World!'
    }
  },
  methods: {
    reverseMessage() {
      this.message = this.message.split('').reverse().join('')
    },
    notify() {
      alert('navigation was prevented.')
    },
    pushMessage(){
      alert('navigation was prevented.')
    }
  }
}
</script>

<template>
  <input v-model="message" placeholder="edit me"><br>
  <button @click="pushMessage()"></button>
  <p>Message is: {{ message }}</p>
</template>

<style>
button, a {
  display: block;
  margin-bottom: 1em;
}
</style>