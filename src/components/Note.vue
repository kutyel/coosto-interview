<template lang="pug">
  .note
    input(type="checkbox" :id="note.id" :checked="note.completed")
    p {{ note.title }}
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
