<template>
  <div id="app">
    <Button />
    <TweetCollection />
  </div>
</template>

<script>
import TweetCollection from './components/TweetCollection.vue';
import Button from './components/Button.vue';

export default {
  name: 'App',
  components: {
    TweetCollection,
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
