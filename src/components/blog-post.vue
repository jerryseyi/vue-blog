<template>
  <div v-show="auth" class="flex flex-col items-center justify-center">
    <div class="max-w-7xl">
      <h3 class="uppercase text-2xl font-bold">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</h3>
      <div class="mt-10">
        <p class="text-xs mt-3">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium ad assumenda cum dicta fugiat, hic laudantium libero molestias, nostrum omnis quae repellendus reprehenderit rerum sapiente vero voluptate voluptates. Ad animi beatae corporis, doloribus eligendi error fuga id impedit iste magnam natus numquam officiis porro quibusdam quisquam suscipit unde veniam voluptatem?
        </p>
        <p class="text-xs mt-3">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Architecto corporis culpa debitis dicta dignissimos dolorem, dolorum eaque enim fuga id minus nam porro quaerat quas quis reprehenderit repudiandae sunt vel velit vero voluptas voluptate voluptatem! Accusamus aut autem consectetur delectus dignissimos, distinctio ea illum molestias nesciunt officiis sint sunt voluptatum? Alias distinctio est id iste libero, minus numquam tenetur velit.
        </p>
      </div>
    </div>

    <div>
      <replies-post></replies-post>
    </div>
  </div>
</template>

<script>
import RepliesPost from "./replies-post.vue";

export default {
  name: "blog-post",
  components: {RepliesPost},
  props: {
    auth: Boolean
  }
}
</script>

<style scoped>

</style>