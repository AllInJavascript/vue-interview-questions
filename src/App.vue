<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <question1></question1>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import question1 from "./components/question1.vue";

export default {
  name: "app",
  components: {
    // HelloWorld
    question1
  },
  data() {
    return {
      testData: {
        name: "xiaomi",
        sex: "男",
        data: [100, 99, 98, 97]
      }
    };
  }
};

/* 

The 'todos' variable inside 'v-for' directive should be replaced with a computed property that returns filtered array instead. You should not mix 'v-for' with 'v-if'

*/
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

li {
  list-style: none;
}
</style>
