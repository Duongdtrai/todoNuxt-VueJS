<template>
  <div>
    <div>
      <h1>List-rendering</h1>
      <form @submit.prevent="addNewTodo">
        <label for="new-todo">Add a todo</label>
        <input
          id="new-todo"
          v-model="newTodoText"
          placeholder="E.g. Feed the cat"
        >
        <button>Add</button>
      </form>
      <ul>
        <li
          v-for="(todo, index) in todos"
          :key="todo.id"
          :content="todo.content"
        >
          <div>
            {{todo.content}}
            <button @click="removeTodotodos(index)">Remove</button>
          </div>
        </li>
      </ul>
    </div>

  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data () {
    return {
      todos: [
        { content: "Máy tính", done: false },
        { content: "Laptop", done: false },
        { content: "Điện thoại", done: false },
      ],
      newTodoText: '',
    };
  },
  methods: {
    removeTodotodos (index) {
      this.todos.splice(index, 1)
    },
    addNewTodo () {
      this.todos.push({
        done: false,
        content: this.newTodoText
      })
      this.newTodoText = ''
    },
  }
}







// List rendering là việc xử lí v-for cùng cách:
// 1. v-if, v-elseif, v-else ( Conditional vuejs)
// 2. template
// 3. computed
// 4. v-show


</script>

