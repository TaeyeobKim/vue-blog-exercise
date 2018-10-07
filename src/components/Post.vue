<template>
  <div class="post">
    <post-component :post='post' />
    <post-comment :comments='post.comments' />
  </div>
</template>

<script>
import PostComponent from './PostContent/PostContent.vue';
import PostComment from './PostContent/PostComments.vue';

export default {
  components: {
    PostComponent,
    PostComment
  },
  props: {
    post: Object
  }
};
</script>

<style scoped>
.post {
  margin: 5%;
  padding: 3%;
  background-color: beige;
  border: 1px solid gainsboro;
  border-radius: 10px;
}
</style>
