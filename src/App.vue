<script>
import BlogPost from "./components/blog-post.vue";

export default {
  name: 'App',
  components: {
    BlogPost
  },
  data() {
    return {
      authenticated: true
    }
  }
}
</script>

<template>
  <div class="flex items-center justify-center flex-col">
    <h3 class="text-3xl flex items-center justify-center mb-10">Welcome to snoopy blog</h3>
    <blog-post :auth="authenticated"></blog-post>
  </div>
</template>

<style scoped>

</style>
