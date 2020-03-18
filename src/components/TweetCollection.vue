<template>
  <div class="container">
    <div id="row-div" class="row">
      <Tweet class="col-lg-3" v-for="tweet in this.tweets" v-bind:key="tweet" :content="tweet" />
    </div>
  </div>
</template>

<script>
import Tweet from "./Tweet.vue";
export default {
  name: "TweetCollection",
  mounted: function() {
    this.$root.$on("heyYouToggle", this.changeStyle);
  },
  components: {
    Tweet
  },
  methods: {
    changeStyle: function() {
      console.log("you clicked a button");
      let div = document.getElementById('row-div');
        if(div.classList == 'row'){
            div.classList.toggle('row', false);
        } else if (div.classList == ''){
            div.classList.toggle('row', true);
        }
    }
  },
  data: function() {
    return {
      tweets: [
        "tweetOne",
        "tweetTwo",
        "tweet three",
        "tweet four",
        "tweet five",
        "tweet six"
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
</style>