<template>
  <header>
    <h1>{{ newTitle }}</h1>
  </header>
</template>

<script>
  export default {
    name: 'Header',
    props: {
      title: String
    },
    data() {
      return {
        name: 'Scott'
      };
    },
    computed: {
      newTitle: function() {
        console.log(this.title);
        console.log(this.name);
        return 'New Title';
      }
    }
}
</script>

<style scoped>
  header {
    background-color: #111;
    padding: 20px;
    color: #fff;
  }

  h1 {
    margin: 0;
  }
</style>
