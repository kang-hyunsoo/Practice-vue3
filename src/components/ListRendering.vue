<template>
  <ul id="array-with-index">
    <li v-for="(item, index) in items">
      {{ parentMessage }} - {{ index }} - {{ item.message }}
    </li>
    <li v-for="n in evenNumbers">{{ n }}</li>
    <li v-for="n in even(numbers)"></li>
  </ul>
</template>

<script>
export default {
  name: "ListRendering",
  data() {
    return {
      parentMessage: 'Parent',
      items: [{ message: 'Foo'}, { message: 'Bar' }],
      numbers: [1, 2, 3, 4, 5, 6]
    }
  },
  computed: {
    evenNumbers() {
      return this.numbers.map(number =>  number + 100)
    }
  },
  methods: {
    even(numbers) {
      return numbers.filter(number => number % 2 === 0)
    }
  }
}
</script>

<style scoped>

</style>