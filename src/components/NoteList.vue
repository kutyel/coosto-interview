<template>
  <div class="hello">
    <ul id="example-1">
      <li v-for="note in notes" :key="note.id">
        <Note :note="note" />
      </li>
    </ul>
    <!-- <pre>{{ JSON.stringify(notes, null, 2) }}</pre> -->
  </div>
</template>

<script>
  import Note from './Note'

  export default {
    name: 'NoteList',
    components: {
      Note
    },
    data () {
      return {
        notes: []
      }
    },
    async created () {
      const res = await fetch('http://weslezw230.230.axc.nl/notes')
      const { data } = await res.json()
      this.notes = data
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1,
  h2 {
    font-weight: normal;
  }

  ul {
    display: flex;
    flex-direction: column;
    align-items: center;
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #42b983;
  }
</style>
