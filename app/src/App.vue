<template>
  <div id="app">
    <button @click="count++">Click me</button>
    <Foo :message="message"/>
  </div>
</template>

<script>
import Foo from 'lib';

export default {
  name: 'app',
  components: {
    Foo
  },
  data: function() {
    return {
      count: 0
    };
  },
  computed: {
    message: function () {
      return `Pressed: ${this.count} times`
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
