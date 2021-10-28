<template>
  <div class="static" :class="{active: isActive, 'text-danger' : hasError}"></div>
<!--  <div class="static active"></div>-->
  <div :class="classObject"></div>
</template>

<script>
export default {
  name: "HtmlClassBinding",
  data() {
    return {
      isActive: true,
      error: null
      }
    },
    computed: {
      classObject() {
        return {
          active: this.isActive && !this.error,
          'text-danger': this.error && this.error.type === 'fatal'
        }
      }
    }

  // data() {
  //   return {
  //     isActive: true,
  //     hasError: false
  //   }
  // }
}
</script>

<style scoped>

</style>