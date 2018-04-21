<template>
  <div id="app">
    <Header :title='title' v-if='isTrue' />
    <MoviesList />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import MoviesList from './components/MoviesList.vue'

export default {
  name: 'app',
  data() {
    return {
      hello: 'Hello World',
      title: 'MovieDB',
      isTrue: true,
      status: 'Loading'
    };
  },
  components: {
    MoviesList,
    Header
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
}
</style>
