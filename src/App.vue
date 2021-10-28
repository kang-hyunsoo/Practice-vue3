<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="This is the Very First Vue Experience " />
  <Counter msg="This is Counter Component"/>
  <ReverseMsg title="This is ReverseMsg" />
  <TypeMsg title="This is TypeMsg" />
  <Conditional title="This is Conditional" />
  <Todo title="This is Todo list"></Todo>
  <Practice></Practice>
  <ListRendering></ListRendering>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Counter from './components/Counter.vue'
import ReverseMsg from "./components/ReverseMsg.vue";
import TypeMsg from "./components/TypeMsg.vue";
import Conditional from "./components/Conditional-rendering.vue"
import Todo from "./components/Todo.vue";
import Practice from './components/Practice.vue';
import HtmlClassBinding from "./components/HtmlClassBinding.vue";
import ListRendering from "./components/ListRendering.vue";

export default {
  name: 'App',
  components: {
    HelloWorld,
    Counter,
    ReverseMsg,
    TypeMsg,
    Conditional,
    Todo,
    Practice,
    HtmlClassBinding,
    ListRendering
  }
}
</script>