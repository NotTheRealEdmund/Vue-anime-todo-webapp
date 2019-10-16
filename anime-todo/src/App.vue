<template>
  <div id="app" class="container">
    <img src="./assets/logo.png" class="logo">
    <todo-list></todo-list>
  </div>
</template>

<script>
import TodoList from './components/TodoList'

export default {
  name: 'App',
  components: {
    TodoList
  }
}
</script>

<style>

.container {
  box-sizing: border-box;
  max-width: 600px;
  margin: 0 auto;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
  font-size: 24px;
}

.logo{
  display: block;
  margin: 20px auto;
  height: 100px;
}

</style>
