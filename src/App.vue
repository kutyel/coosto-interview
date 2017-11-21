<template>
  <div id="app">
    <h1>TODO's</h1>
    <NoteList />
  </div>
</template>

<script>
  import NoteList from './components/NoteList'

  export default {
    name: 'app',
    components: {
      NoteList
    }
  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
