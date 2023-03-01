<template>
  <div>
    <ul class="mt-5">
      <li v-for="reply in replies" :key="reply.id" class="mb-5">
        {{ reply.title }} -> {{ reply.body}}
      </li>
    </ul>

    <reply-post @fromReply="checkReply"></reply-post>
  </div>
</template>

<script>
import ReplyPost from "./reply-post.vue";

export default {
  name: "replies-post",
  components: {ReplyPost},
  data() {
    return {
      replies: [
        {id: 0, name: 'John Doe', title: 'A short reply', body: 'Just saying my mind'},
        {id: 1, name: 'Jane Doe', title: 'A short reply 1', body: 'Just saying my mind 1'},
        {id: 2, name: 'Mary Doe', title: 'A short reply 2', body: 'Just saying my mind 2'},
        {id: 3, name: 'Hills Doe', title: 'A short reply 3', body: 'Just saying my mind 3'},
        {id: 4, name: 'Gilbert Doe', title: 'A short reply 4', body: 'Just saying my mind 4'},
      ]
    }
  },

  methods: {
    checkReply(data) {
      this.replies.push(data);
    }
  }
}
</script>

<style scoped>

</style>