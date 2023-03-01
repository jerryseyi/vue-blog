<template>
  <div v-show="auth" class="flex items-center justify-center">
    <div class="max-w-7xl">
      <h3 class="uppercase text-2xl font-bold">Lorem ipsum dolor sit amet, consectetur adipisicing elit.</h3>
    </div>
  </div>
</template>

<script>
export default {
  name: "blog-post",
  props: {
    auth: Boolean
  }
}
</script>

<style scoped>

</style>