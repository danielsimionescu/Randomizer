<template>
<v-container>
  <div class="text-xs-center">
    <result :result="result"></result>
    <v-btn color="teal" dark @click="randomize">Randomize</v-btn>
  </div>
  <v-layout row>
    <list v-for="group in groups" :key="group.type" :group="group"></list>
  </v-layout>
</v-container>
</template>

<script>
import List from './List'
import Result from './Result'

import data from '../data.js'

export default {
  name: 'Home',
  components: {
    List,
    Result
  },
  data () {
    return {
      groups: [],
      result: []
    }
  },
  created () {
    this.groups = data;
  },
  methods: {
    randomize() {
      this.result = [];

      this.groups.forEach(group => {
        let rand = group.items[Math.floor(Math.random() * group.items.length)];
        this.result.push(rand);
      });
    }
  }
}
</script>

<style scoped>
</style>
