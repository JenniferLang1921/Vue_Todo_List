<template>
  <header class="header">
    <h1>TodoList</h1>
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>
  .header {
    background: #2A0E3F;
    color: #fff;
    text-align: center;
    padding: 10px;
    margin-top: -10px;
  }
  .header a {
    color: #fff;
    padding-right: 5px;
    text-decoration: none;
  }

   .header a:hover {
    color: #C9E9F4;
    text-decoration: underline;
  }

    
</style>