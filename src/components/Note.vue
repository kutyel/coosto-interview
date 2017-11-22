<template>
  <div :class="{ completed: note.completed }">
    <input type="checkbox" :id="note.id" :checked="note.completed" />
    <label>{{ note.title }}</label>
  </div>
</template>

<script>
  export default {
    name: 'Note',
    props: ['note']
  }
</script>

<style scoped>
  input {
    text-align: center;
    width: 40px;
    height: 40px;
    position: absolute;
  }

  label {
    white-space: pre-line;
    word-break: break-all;
    padding: 15px 60px 15px 15px;
    margin-left: 45px;
    display: block;
    line-height: 1.2;
    transition: color 0.4s;
  }

  .completed {
    color: #d9d9d9;
    text-decoration: line-through;
  }

  input::input-placeholder {
    font-style: italic;
    font-weight: 300;
    color: #e6e6e6;
  }
</style>
