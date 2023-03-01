<template>
  <div>
    <form action="" class="flex flex-col">
      <input type="text" class="mb-2 border border-2" placeholder="id" v-model="reply.id">
      <input type="text" class="mb-2 border border-2" placeholder="name" v-model="reply.name">
      <input type="text" class="mb-2 border border-2" placeholder="title" v-model="reply.title">
      <input type="text" class="mb-2 border border-2" placeholder="body" v-model="reply.body">

      <a href="#" @click.prevent="submit">submit</a>
    </form>
  </div>
</template>

<script>
export default {
  name: "reply-post",
  data() {
    return {
      reply: {
        id: null,
        name: null,
        title: null,
        body: null
      }
    }
  },

  methods: {
    submit() {
      this.$emit('fromReply', this.reply)
    }
  }
}
</script>

<style scoped>

</style>