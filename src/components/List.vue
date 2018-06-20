<template>
  <v-layout>
    <item v-for="i in 10" :key="i"></item>
  </v-layout>
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
  
</style>
