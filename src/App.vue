<template>
  <div id="app">
    <img src="./assets/logo.png">
    <hello></hello>
    {{ hhh }}
    {{ object.FirstName }}
    <template v-if="loginType === 'username'">
      <label>Username</label>
      <input placeholder="Enter your username">
    </template>
    <template v-else>
      <label>Email</label>
      <input placeholder="Enter your email address">
    </template>
  </div>
</template>

<script>
import Hello from './components/Hello'
console.log();
export default {
  name: 'app',
  components: {
    Hello
  },
  data:function() {
    return {
      hhh:'哈哈哈啊啊啊啊啊啊啊啊啊啊啊啊啊啊啊啊啊啊啊实打实啊',
      object: {
        FirstName: 'John',
        LastName: 'Doe',
        Age: 30
      }
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
