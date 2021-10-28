<template>
  <h1>{{ title }}</h1>
  <h3>{{ msg }}</h3>
  <button v-on:click="reverseMessage">Reverse Message</button>
</template>

<script>
export default {
  name: "ReverseMsg",
  props: {
    title: String
  },
  data() {
    return {
      msg: 'Make the message reversed'
    }
  },
  methods: {
    reverseMessage() {
      this.msg = this.msg
          .split('')
          .reverse()
          .join('')
    }
  }
}
</script>

<style scoped>

</style>