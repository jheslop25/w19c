<template>
  <div id="app">
    <Button />
    <Tweet />
  </div>
</template>

<script>
import Tweet from './components/Tweet.vue';
import Button from './components/Button.vue';

export default {
  name: 'App',
  components: {
    Tweet,
    Button
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
