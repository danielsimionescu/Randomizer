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
      result: {}
    }
  },
  created () {
    this.groups = data;
  },
  methods: {
    randomize() {
      alert("randomize");

      // get one random from each
      // add them in an array (4)
    }
  }
}
</script>

<style scoped>
</style>
