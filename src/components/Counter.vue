<template>
  <h1>{{ msg }}</h1>
  <button v-on:click="count++">click counter</button>
  <h3>{{ count }}</h3>
  <p>GO AHEAD VUE !!</p>
</template>

<script>
export default {
  name: "Counter",
  props: {
    msg: String
  },

  data() {
    return {
      count: 0
    }
  }
}
</script>


