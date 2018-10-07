<template>
  <div class="comment-box">
    <h4>댓글</h4>
    <ol>
      <li v-for="comment in comments" :key="comment.id">{{comment.body}}</li>
    </ol>
  </div>
</template>

<script>
export default {
  props: {
    comments: Array
  }
};
</script>

<style scoped>
.comment-box {
  margin-top: 20px;
}
</style>
