<template>
  <div class="content-box">
    <h2>{{post.title}}</h2>
    <div>{{post.body}}</div>
    <div class="timestamp">{{post.created_at}}</div>
  </div>
</template>

<script>
export default {
  props: {
    post: Object
  }
};
</script>

<style scoped>
.content-box > * {
  padding: 10px;
}

.timestamp {
  text-align: right;
}
</style>
