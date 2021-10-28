<template>
  <span :style="styleObject">KAYA JAM</span>
<!--  <span :style="{ color: '#FFD679',  fontWeight: '800'}">{{fullName}}</span>-->
<!--  <p>published or not :</p>-->
<!--  <div>{{ this.author.books.length > 0 ? 'yep' : 'nope'}}</div>-->
  <div v-if="Math.floor(Math.random()*10) > 5">View is awesome!</div>
  <div v-else-if="Math.floor(Math.random()*10) === 5">You are lucky!</div>
  <div v-else>Oh No:(</div>
</template>

<script>
export default {
  name: "Practice",
  props: String,
  data() {
    // return {
    //   author: {
    //     name: 'Kaya',
    //     books: [
    //         'Getting close to Vue3',
    //         'Deep dive CSS'
    //     ]
    //   }
    // }
    // return {
    //   firstName: 'Kang',
    //   lastName: 'Kaya',
      // fullName: 'Kaya Kang'
    //}
    return {
      styleObject: {
        color: 'rosybrown',
        fontSize: '3rem',
        fontWeight: 'bold'
      }
    }
  },
  computed: {
    fullName: {
      //getter
      get() {
        return this.firstName + ' ' + this.lastName
      },
      //setter
      set(newValue) {
        const names = newValue.split('')
        this.firstName = names[0]
        this.lastName -= names[names.length - 1]
      }
    }
  }
}

</script>

<style scoped>

</style>