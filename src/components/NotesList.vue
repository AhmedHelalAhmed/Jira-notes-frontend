<template>
  <div class="container">
    <h1>list of notes</h1>

    <b-list-group>
      <b-list-group-item v-for="(note, index) in notes" v-bind:key="index">{{
        note.subject
      }}</b-list-group-item>
    </b-list-group>
  </div>
</template>

<script>
export default {
  name: "NotesList",
  props: {
    msg: String,
  },
  data() {
    return {
      notes: [{ subject: "task1" }, { subject: "task2" }, { subject: "task3" }],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
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
