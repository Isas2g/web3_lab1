<template>
  <div id="app">
    <div id="nav">
      <Header />
    </div>
    <div class="content">
      <router-view/>
    </div>
    <Footer />
  </div>
</template>

<script>
  import Header from '@/components/Header.vue';
  import Footer from '@/components/Footer.vue';

  export default {
    name: 'App',
    components: {
      Footer,
      Header
    }
  }
</script>

<style>

body {
  margin: 0;
}

html,
body {
  height: 100%;
}

#app {
  text-align: center;
  color: #2c3e50;
  min-height: 100%;
  display: flex;
  flex-direction: column;
}

.content {
  flex: 1 1 auto;
}
</style>
