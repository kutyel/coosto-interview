<template>
  <div id="app">
    <h1>todos</h1>
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
  html,
  body {
    margin: 0;
    padding: 0;
    background: #f5f5f5;
    font-size: 2rem;
  }

  :focus {
    outline: 0;
  }

  #app {
    font: 14px 'Helvetica Neue', Helvetica, Arial, sans-serif;
    line-height: 1.4em;
    color: #4d4d4d;
    min-width: 230px;
    max-width: 550px;
    margin: 300 auto;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    font-weight: 300;
    background: #fff;
    margin: 130px 0 40px 0;
    position: relative;
    box-shadow: 0 2px 4px 0 rgba(0, 0, 0, 0.2),
                0 25px 50px 0 rgba(0, 0, 0, 0.1);
  }

  h1 {
    position: absolute;
    top: -155px;
    width: 100%;
    font-size: 100px;
    font-weight: 100;
    text-align: center;
    color: rgba(175, 47, 47, 0.15);
    text-rendering: optimizeLegibility;
  }
</style>
