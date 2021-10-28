<template>
  <h1>{{ title }}</h1>
  <h3>{{ message }}</h3>
  <input v-model="message" placeholder="Write here" />
</template>

<script>
export default {
  name: "TypeMsg",
  props: {
    title: String
  },
  data() {
    return {
      message: ''
    }
  },
}
</script>

<style scoped>

</style>