<template>
  <div>
    <form @submit.prevent="addTodo">
      <input type="text" v-model="title" name="title" placeholder="Add to do item...">
      <input type="submit" value="Submit" class="btn">
    </form>
  </div>
</template>

<script>
// import uuid from 'uuid';
export default {
  name: "AddTodo",
  data() {
    return {
      title: '',
    }
  },
  methods: {
    addTodo() {
      const newTodo = {
        title: this.title,
        completed: false
      }
      // Send up to parent
      this.$emit('add-todo', newTodo);
      this.title = '';
    }
  }
}
</script>

<style scoped>
  form {
    display: flex;
  }
  input[type="text"] {
    flex: 10;
    padding: 5px;
    font-size: 150%;
    margin: 5% 0 5% 5%;
  }
  input[type="submit"] {
    flex: 2;
    margin: 5% 5% 5% 0;
  }
</style>
