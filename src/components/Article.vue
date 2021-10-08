<template>
  <main>
    <h1>Article «{{news[id-1].name}}»</h1>
    <div class='article'>
        {{news[id-1].desc}}
    </div>
  </main>
</template>

<script>
import news from '@/assets/articles.json'

export default {
  name: 'Article',
  props: ['id'],
  data(){
      return {
        news: news
    };
  }
}
</script>

<style scoped>
.article {
    padding: 8px;
}
</style>