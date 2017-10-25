<template>
  <div>
    <input type="checkbox" name="done" :id="note.id" :checked="note.completed">
    <p>{{ note.title }}</p>
  </div>
</template>

<script>
  export default {
    name: 'Note',
    props: ['note']
  }
</script>

<style>
  p {
    display: inline-block;
  }
</style>
