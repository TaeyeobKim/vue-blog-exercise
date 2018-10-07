<template>
  <div id="app">
    <post v-for="post in posts" :key="post._id" :post="post" />
  </div>
</template>

<script>
import Post from './components/Post.vue';
import posts from '../blogdata';

export default {
  name: 'app',
  components: {
    Post
  },
  data() {
    return {
      posts
    };
  }
};
</script>

<style>
#app {
  margin: 10%;
}
</style>
