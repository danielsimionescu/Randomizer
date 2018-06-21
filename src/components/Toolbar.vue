<template>
  <v-toolbar color="teal" dark>
    <v-toolbar-title>{{title | uppercase}}</v-toolbar-title>
    <v-toolbar-items class="hidden-sm-and-down">
      <v-btn flat>Web</v-btn>
      <v-btn flat>Mobile</v-btn>
      <v-btn flat>Tools</v-btn>
    </v-toolbar-items>
    <v-spacer></v-spacer>
    <v-toolbar-items class="hidden-sm-and-down">
      <v-btn flat>Repo</v-btn>
      <v-btn flat>YouTube</v-btn>
      <v-btn flat>GitHub</v-btn>
    </v-toolbar-items>
  </v-toolbar>
</template>

<script>
export default {
  name: "Toolbar",
  data () {
    return {
      title: 'Randomizer'
    }
  },
  filters: {
    uppercase(value) {
      return value.toUpperCase();
    }
  }
};
</script>

<style>
</style>
