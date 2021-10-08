<template>
  <main>
    <h1>News</h1>
    <div>
      <div v-for="(article, index) in news" :key="index">
        <h2><router-link :to='"/article/" + article.id'>{{article.id}} {{article.name}}</router-link></h2>
        <p>{{article.shortDesc}}</p>
      </div>
    </div>
  </main>
</template>

<script>
import news from '../assets/articles.json'

export default {
  name: 'News',
  data(){
      return {
        news
    };
  }
}
</script>

<style scoped>

</style>