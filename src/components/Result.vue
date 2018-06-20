<template>
  <v-card>
    <v-avatar
      class="logo"
      v-for="i in 4"
      :key="i"
      :tile="true"
      size="130"
    >
      <img src="https://cdn.worldvectorlogo.com/logos/angular-icon-1.svg" alt="avatar">
    </v-avatar>
  </v-card>
</template>

<script>
export default {
  name: 'result',
}
</script>

<style scoped>
  .logo {
    margin: 15px;
  }
</style>
