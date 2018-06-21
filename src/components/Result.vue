<template>
  <v-card>
    <v-avatar
      class="logo"
      v-for="item in result"
      :key="item.name"
      :tile="true"
      size="130"
    >
      <img :src="item.logo" alt="avatar">
    </v-avatar>
  </v-card>
</template>

<script>
export default {
  name: 'result',
  props: ['result']
}
</script>

<style scoped>
  .logo {
    margin: 15px;
  }
</style>
