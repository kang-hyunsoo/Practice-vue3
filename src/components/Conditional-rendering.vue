<template>
  <h1>{{ title }}</h1>
  <button @click="switchSeen">Click to see</button>
  <span v-if="seen">Now you can see me!</span>
</template>

<script>
export default {
  name: "Conditional",
  props: {
    title: String
  },
  data() {
    return {
      seen: false
    }
  },
  methods: {
    switchSeen() {
      this.seen === true ? this.seen = false : this.seen = true
      // 클릭하면 true false 변경할 수 있게 만들어보기 =
    }
  }
}
</script>

