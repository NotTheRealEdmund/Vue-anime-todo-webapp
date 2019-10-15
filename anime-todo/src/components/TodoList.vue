<template>
  <div>
    <input type="text" class="todo-input" placeholder="Watch an anime" v-model="newTodo">
    <div v-for="todo in todos" :key="todo.id" class="todo-item">
      {{ todo.title }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'todo-list',
  data () {
    return {
      newTodo: '',
      todos: [
        {
          'id': 1,
          'title': 'Yuru Yuri',
          'completed': false,
        },
        {
          'id': 2,
          'title': 'Seitokai Yakuindomo',
          'completed': false,
        },
        {
          'id': 3,
          'title': 'Joshiraku',
          'completed': false,
        }
      ]
    }
  }
}
</script>

<style lang="scss">
  .todo-input {
    width: 100%;
    padding: 10px 18px;
    font-size: 18px;
    margin-bottom: 16px;

    &:focus {
      outline: 0;
    }
  }
</style>