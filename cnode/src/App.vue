<template>
  <div id="app">
    <Header></Header>
    <div class = "main">
      <router-view name = "slidebar"></router-view>
      <router-view name = "main"></router-view>
    </div>

  </div>
</template>

<script>
  import Header from './components/Header'
  import PostList from "./components/PostList";
  export default {
    name: 'App',
    components: {
      Header,PostList
    }
  }
</script>

<style>
  * {
    margin: 0;
    padding: 0;
  }
  #app {

    width: 100%;
    height: 100%;
    background: #ccc;
  }
  .main {
    width: 80%;
    margin: 0 auto;
  }
</style>
