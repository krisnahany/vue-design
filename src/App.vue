<template>
  <div id="app">
    <div class="container">
      <Menu></Menu>
      <Video></Video>
    </div>
  </div>
</template>

<script>
import Menu from './components/Menu'
import Video from './components/Video.vue'

export default {
  name: 'App',
  components: {
    Menu,
    Video
  }
}
</script>

<style>
#app {
  font-family: Roboto, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.container {
  background-color: #F8F9FA;
  border: 1px solid #888888;
  box-shadow: 5px 10px 18px #888888;
}

button {
  border: none;
  background: none;
}

.left {
  float: left;
}

.right {
  float: right;
}
</style>
