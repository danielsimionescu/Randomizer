<template>
  <v-flex>
    <v-card class="card">
      <v-avatar
        :tile="true"
        size="120"
      >
        <img src="https://vuejs.org/images/logo.png" alt="avatar">
      </v-avatar>
      <v-card-title primary-title>
        <h3 class="headline mb-0">Vue.js</h3>
      </v-card-title>
    </v-card>
  </v-flex>
</template>

<script>
export default {
  name: 'Item'
}
</script>

<style>
.card {
    padding: 0 10px 0 10px;
    margin-right: 8px;
  }
</style>
