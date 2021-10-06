<template>
  <div id="app">
    <img src="./assets/logo.png">
    <HelloWorld/>
    <PostsList/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld';
import PostsList from './components/PostsList';

export default {
  name: 'App',
  components: {
    HelloWorld,
    PostsList
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
