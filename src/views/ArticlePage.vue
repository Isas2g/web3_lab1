<template>
  <div id="app">
    <Article v-bind:id="$route.params.id" />
  </div>
</template>

<script>
import Article from '@/components/Article.vue';

export default {
  name: 'Home',
  components: {
    Article
  }
}
</script>

<style>


body {
  font-family: 'Roboto';
}

</style>
