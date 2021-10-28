<template>
  <h1>{{ title }}</h1>
  <ul>
    <li v-for="todo in todos">
      {{ todo.text }}
    </li>
  </ul>
</template>

<script>
export default {
  name: "Todo",
  props: {
    title : String
  },
  data() {
    return {
      todos: [
        { text: 'Learn Vue3'},
        { text: 'Tea time with Joa and Siwan'},
        { text: 'English study'}
      ]
    }
  }
}
</script>

<style scoped>

</style>