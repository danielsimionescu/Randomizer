<template>
<v-card>
  <h2 class="headline">Frontend</h2>
  <v-container fluid grid-list-xs>
    <v-layout row wrap class="list">
      <item v-for="i in 20" :key="i"></item>
    </v-layout>
  </v-container>
</v-card>
</template>

<script>
import Item from './Item'

export default {
  name: 'List',
  components: {
    Item
  }
};
</script>

<style scoped>
  .list {
    margin-bottom: 10px;
  }
</style>
