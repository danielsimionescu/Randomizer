<template>
  <v-card>
    <item v-for="item in result" :key="item.name" :item="item"></item>
  </v-card>
</template>

<script>
import Item from './Item';

export default {
  name: 'result',
  props: ['result'],
  components: {
    Item
  }
}
</script>

<style scoped>

</style>
