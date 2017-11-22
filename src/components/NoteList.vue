<template>
    <ul>
      <li v-for="note in notes" :key="note.id">
        <Note :note="note" />
      </li>
    </ul>
</template>

<script>
  import Note from './Note'

  export default {
    name: 'NoteList',
    components: { Note },
    data: () => ({ notes: [] }),
    async created () {
      const res = await fetch('http://weslezw230.230.axc.nl/notes')
      const { data } = await res.json()
      this.notes = data
    }
  }
</script>

<style scoped>
  ul {
    display: flex;
    flex-direction: column;
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }
</style>
